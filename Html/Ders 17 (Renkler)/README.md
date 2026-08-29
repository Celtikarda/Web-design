# 📚 Ders 17

## 🎯 Konu

Renkler

---

## 📖 Öğrendiğim Kavramlar

* RGB = "Red Green Blue" kelimelerinden gelir.
* RGB'de her renk kanalı `0-255` arasında değer alır.
* HEX = Renkleri `#` işareti ve hexadecimal sayı sistemiyle ifade eder.
* HSL = "Hue, Saturation, Lightness" kelimelerinden gelir.
* `color` yazının rengini belirler.
* `background-color` elementin arka plan rengini belirler.
* RGBA, RGB'ye ek olarak saydamlık değeri (`alpha`) içerir.

---

## 📝 Sözdizimi (Syntax)

```CSS
color: red;

color: #ff0000;

color: rgb(255, 0, 0);

color: rgba(255, 0, 0, 0.5);

color: hsl(0, 100%, 50%);

background-color: yellow;
```

---

## 💡 Mantığı

RGB'de üç farklı renk kanalı bulunur:

* `R` → Kırmızı
* `G` → Yeşil
* `B` → Mavi

Her kanal `0-255` arasında değer alabilir.

Örneğin:

```CSS
rgb(255, 0, 0)
```

→ Kırmızı

```CSS
rgb(0, 255, 0)
```

→ Yeşil

```CSS
rgb(0, 0, 255)
```

→ Mavi

```CSS
rgb(255, 255, 255)
```

→ Beyaz

```CSS
rgb(0, 0, 0)
```

→ Siyah

HEX renkleri `#` ile başlar ve hexadecimal sistem kullanır.

HSL ise rengi; renk tonu, doygunluk ve açıklık üzerinden ifade eder.

---

## ⚠️ Dikkat Edilmesi Gerekenler

* RGB'de değerler `0-255` arasında olmalıdır.
* HEX kodlarının başında `#` bulunur.
* `color` ile yazı rengini, `background-color` ile arka plan rengini değiştiririz.
* RGB ile RGBA aynı değildir; RGBA'da ayrıca saydamlık değeri bulunur.

---

## ❌ Yaptığım Hatalar

* RGB'deki değerlerin `0-255` arasında olduğunu ilk başta bilmiyordum.
* Renkleri sadece isimleriyle ifade edebileceğimi düşünüyordum.

---

## ✅ Doğru Kullanım

```HTML
<p style="color: rgb(255, 0, 0);">
    Kırmızı yazı
</p>

<p style="background-color: #ffff00;">
    Sarı arka plan
</p>
```

---

## 🧪 Bu Derste Yazdığım Örnekler

* `rgb(255, 0, 0)` → Kırmızı
* `rgb(0, 255, 0)` → Yeşil
* `rgb(0, 0, 255)` → Mavi
* `rgb(255, 255, 255)` → Beyaz
* `rgb(0, 0, 0)` → Siyah
* `rgba(255, 0, 0, 0.5)` → Yarı saydam kırmızı

---

## 🧠 Kendime Notlar

> RGB = Red + Green + Blue
> Her RGB kanalı = `0-255`
> HEX = `#` + hexadecimal renk kodu
> HSL = Hue + Saturation + Lightness
> `color` = yazı rengi
> `background-color` = arka plan rengi

---

## 🔥 Bir Sonraki Hedef

CSS renklerini daha iyi kullanmak için **HEX, RGB ve HSL arasındaki farkları öğrenmek ve renk değerlerini kendim oluşturabilmek.**
