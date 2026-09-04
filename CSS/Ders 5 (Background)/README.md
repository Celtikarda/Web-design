# 📚 Ders 5

## 🎯 Konu

Background özellikleri

---

## 📖 Öğrendiğim Kavramlar

- background-position: center; = Arka plan resminin konumunu belirler. (`center`, `top`, `bottom`, `left`, `right` vb. kullanılabilir.)

- background-repeat: no-repeat; = Arka plan resminin tekrarlanmamasını sağlar.

- background-repeat: repeat; = Arka plan resminin hem yatay hem dikey eksende tekrarlanmasını sağlar.

- `background-repeat: repeat-x;` = Arka plan resminin yalnızca yatay eksende tekrarlanmasını sağlar.

- `background-repeat: repeat-y;` = Arka plan resminin yalnızca dikey eksende tekrarlanmasını sağlar.

- `background-repeat: no-repeat repeat;` = İlk değer yatay, ikinci değer dikey tekrarı belirler. Bu nedenle yatayda tekrarlanmaz, dikeyde tekrarlanır.

- `background-size: cover;` = Arka plan resmini kapsayıcı alanı tamamen kaplayacak şekilde boyutlandırır. Resmin bazı kısımları kesilebilir.

- `background-size: contain;` = Arka plan resminin tamamını gösterecek şekilde boyutlandırır. Resim kesilmez ancak boş alan kalabilir.

- `background-attachment: fixed;` = Arka plan resminin sayfa kaydırılırken sabit kalmasını sağlar.

- `background-attachment: local;` = Arka planın, bulunduğu elementin içeriği kaydırıldığında içerikle birlikte hareket etmesini sağlar.

- `background-attachment: scroll;` = Arka planın element ile birlikte hareket etmesini sağlar. Sayfa kaydırıldığında arka plan sabit kalmaz.

- `background-color: ;` = Elementin arka plan rengini belirler.

- `background-image: url("");` = Elementin arka planına resim ekler.

---

## 📝 Sözdizimi

```css
body {
    background-color: black;
    background-image: url("resim.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
}
```

---

## 💡 Mantığı

`background` özelliklerini bir arka plan resmini **kontrol etmek** gibi düşünebilirim.

- **Nerede duracak?** → `background-position`
- **Tekrarlanacak mı?** → `background-repeat`
- **Ne kadar büyüyecek?** → `background-size`
- **Sayfayı kaydırınca hareket edecek mi?** → `background-attachment`
- **Arka plan rengi ne olacak?** → `background-color`
- **Hangi resim kullanılacak?** → `background-image`

---

## ⚠️ Dikkat

- `background-position: fixed;` **yanlış kullanımdır.** Sabitlemek için `background-attachment: fixed;` kullanılır.

- `scroll` kelimesinin doğru yazımı **`scroll`** şeklindedir, `scrool` değildir.

- `cover` resmin tamamını göstermek zorunda değildir. Alanı tamamen doldurmak için resmin bir kısmını kesebilir.

- `contain` resmin tamamını gösterir ancak kapsayıcıda boş alan bırakabilir.

---

## ❌ Yaptığım Hatalar

- `background-position: fixed;` yazdım. Doğrusu: `background-attachment: fixed;`

- `scrool` yazdım. Doğrusu: `scroll`

---

## 🧪 Örnekler

### 1. Resmi tekrar ettirmemek

```css
body {
    background-image: url("resim.jpg");
    background-repeat: no-repeat;
}
```

### 2. Resmi tüm alanı kaplayacak şekilde yapmak

```css
body {
    background-image: url("resim.jpg");
    background-size: cover;
}
```

### 3. Arka planı sabitlemek

```css
body {
    background-image: url("resim.jpg");
    background-size: cover;
    background-attachment: fixed;
}
```

### 4. Arka planı ortalamak

```css
body {
    background-image: url("resim.jpg");
    background-position: center;
}
```

---

## 🧠 Kendime Not

`background` özelliklerinde her özellik farklı bir şeyi kontrol eder.

**position = konum**
**repeat = tekrar**
**size = boyut**
**attachment = hareket/sabitlik**
**color = renk**
**image = resim**

Özellikle `cover` ile `contain` arasındaki farkı unutmamalıyım:

**cover → alanı tamamen doldurur, resmi kesebilir.**

**contain → resmi tamamen gösterir, boş alan bırakabilir.**

---

## 🔥 Bir Sonraki Hedef

**CSS `background` shorthand özelliğini öğrenmek.**

Birden fazla `background` özelliğini tek satırda kullanmayı öğren:
`background: ...;`

Ardından `linear-gradient()` ve arka plan üzerinde **gradient kullanımı** konusuna geç.
