# Sabit Menü Örneği

Bu proje, CSS `position: fixed` kullanılarak oluşturulmuş basit bir sabit üst menü örneğidir.

Sayfa aşağı doğru kaydırılsa bile siyah menü ekranın üst kısmında sabit kalır.

## Kullanılan Yapılar

- HTML
- CSS
- `position: fixed`
- `margin`
- `padding`
- `border-radius`

## Özellikler

- Menü siyah arka plana ve beyaz yazıya sahiptir.
- Menü ekranın en üstüne sabitlenmiştir.
- Sayfa kaydırılırken menü görünmeye devam eder.
- İçerik, menünün altında başlayacak şekilde boşluk bırakır.

## Önemli CSS Kodları

```css
.navbar {
    position: fixed;
    top: 0px;
    left: 0px;
}
```

`position: fixed`, menüyü sayfaya değil doğrudan ekran penceresine sabitler.

```css
top: 0px;
left: 0px;
```

Menünün ekranın üst ve sol kenarından başlamasını sağlar.

```css
.yazi {
    margin-top: 50px;
}
```

Sabit menü normal sayfa akışından çıktığı için içerik menünün altında kalabilir. Bu kod, yazıları aşağı kaydırarak menünün altında görünmesini sağlar.

## Çalıştırma

1. Kodu `index.html` adıyla kaydet.
2. Dosyaya çift tıklayarak tarayıcıda aç.
3. Sayfayı aşağı kaydır.
4. Menünün ekranın üstünde sabit kaldığını gözlemle.

## Geliştirilebilir Fikirler

- Menüye bağlantılar eklemek
- Menü yüksekliğini artırmak
- `display: flex` ile menü öğelerini yatay hizalamak
- Mobil ekranlar için responsive tasarım eklemek