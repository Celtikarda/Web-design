# 📚 Ders 18 — Meta Etiketi

## 🎯 Konu

HTML'de `<meta>` etiketi ve sayfa hakkında bilgi verme.

---

# 📖 Öğrendiğim Kavramlar

### 1. `<meta>` etiketi nedir?

`<meta>` etiketi, HTML sayfasının kendisi hakkında **metadata (üst veri)** vermek için kullanılır.

Metadata'yı şöyle düşünebilirim:

> Kullanıcıya gösterilen asıl içerik değil, sayfa hakkında tarayıcıya ve diğer sistemlere verilen bilgiler.

Örneğin:

```html
<meta charset="UTF-8">
```

Bu etiket sayfada görünmez.

Tarayıcı bu bilgiyi okuyarak HTML dosyasındaki karakterlerin nasıl yorumlanacağını anlar.

---

### 2. `<meta>` nerede kullanılır?

Genellikle `<head>` içerisinde kullanılır.

```html
<!DOCTYPE html>

<html lang="tr">

<head>

    <meta charset="UTF-8">

</head>

<body>

    <h1>Merhaba</h1>

</body>

</html>
```

Burada:

```html
<head>
```

sayfanın kullanıcıya doğrudan gösterilmeyen ayarlarının ve bilgilerinin bulunduğu bölümlerden biridir.

`<meta>` de genellikle burada bulunur.

---

### 3. `<meta>` kapanış etiketi almaz

Şöyle yazılmaz:

```html
<meta></meta>
```

Doğru kullanım:

```html
<meta charset="UTF-8">
```

Yani `<meta>` bir **void element**tir.

---

# 🔤 charset

En önemli meta kullanımlarından biridir.

```html
<meta charset="UTF-8">
```

Buradaki:

```text
charset
```

→ **character set (karakter kodlaması)** anlamına gelir.

`UTF-8` ise kullanılan karakter kodlamasıdır.

Örneğin Türkçedeki:

```text
ç
ğ
ı
İ
ö
ş
ü
```

gibi karakterlerin doğru şekilde yorumlanmasına yardımcı olur.

Bu yüzden HTML belgelerinde genellikle:

```html
<meta charset="UTF-8">
```

kullanırız.

### Mantığı

Tarayıcı HTML dosyasını okurken karakterlerin nasıl kodlandığını bilmelidir.

UTF-8 kullanmak, çok geniş bir karakter kümesini desteklediği için modern web sayfalarında standart tercihtir.

---

# 📱 viewport

Mobil uyumluluk açısından çok önemli bir kullanımdır.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Bu satırı parçalayalım.

---

## `name="viewport"`

Burada:

```html
name="viewport"
```

meta bilgisinin **viewport** ile ilgili olduğunu belirtir.

Viewport'u basitçe:

> Kullanıcının web sayfasını görüntülediği ekran alanı

olarak düşünebilirim.

---

## `content="width=device-width"`

Buradaki:

```html
width=device-width
```

sayfanın görüntü genişliğinin cihazın ekran genişliğine göre ayarlanmasını ister.

Örneğin telefon ekranı dar ise sayfanın genişliği de buna göre ele alınır.

---

## `initial-scale=1.0`

Bu:

```html
initial-scale=1.0
```

sayfanın ilk açılışındaki başlangıç ölçeğini belirtir.

`1.0` → normal başlangıç ölçeği.

---

# 📝 name ve content

Şu yapıyı sık sık göreceğim:

```html
<meta name="..." content="...">
```

Burada:

```html
name
```

→ Verdiğimiz meta bilginin **türünü/adını** belirtir.

```html
content
```

→ O bilgiye ait **değeri/içeriği** belirtir.

Örneğin:

```html
<meta name="description" content="HTML öğreniyorum.">
```

Burada:

```text
name = description
content = HTML öğreniyorum.
```

Yani:

> Meta bilgisinin türü description, değeri ise "HTML öğreniyorum."

---

# 🔎 description

Sayfanın açıklamasını belirtmek için kullanılır.

```html
<meta name="description" content="HTML öğreniyorum ve web geliştirme çalışıyorum.">
```

Burada:

```text
name
```

→ `description`

ve:

```text
content
```

→ sayfanın açıklaması.

Bu bilgi arama motorları tarafından bazı durumlarda arama sonuçlarında açıklama olarak kullanılabilir.

Ancak arama motorları her zaman verdiğimiz açıklamayı aynen göstermek zorunda değildir.

---

# 👤 author

Sayfanın yazarını belirtmek için kullanılabilir.

```html
<meta name="author" content="Eyüp Arda">
```

Burada:

```text
name = author
content = Eyüp Arda
```

anlamına gelir.

---

# 🔑 keywords

Sayfayla ilgili anahtar kelimeler belirtilebilir.

```html
<meta name="keywords" content="HTML, CSS, JavaScript">
```

Burada:

```text
HTML
CSS
JavaScript
```

sayfayla ilişkili anahtar kelimeler olarak belirtilmiştir.

### Önemli:

`keywords` etiketini öğrenmek HTML açısından faydalıdır.

Ancak modern arama motorlarında SEO açısından **eskisi kadar önemli değildir**.

Yani:

> `keywords` kullanınca Google'da otomatik olarak üst sıralara çıkmam.

---

# ⚙️ http-equiv

Bir başka meta kullanım şeklidir:

```html
<meta http-equiv="...">
```

`http-equiv`, tarayıcıya bazı HTTP başlıklarıyla ilişkili talimatlar vermek için kullanılabilir.

Örneğin:

```html
<meta http-equiv="refresh" content="5">
```

Bu, sayfanın belirli bir süre sonra yenilenmesini sağlayabilir.

Ancak günlük HTML çalışmalarımda bunu sürekli kullanmam gerekmez.

Öncelikle:

```html
charset
viewport
description
```

gibi temel kullanımları öğrenmem daha önemlidir.

---

# 📝 Sözdizimi (Syntax)

### charset

```html
<meta charset="UTF-8">
```

---

### viewport

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

### description

```html
<meta name="description" content="Sayfanın açıklaması">
```

---

### author

```html
<meta name="author" content="Sayfanın yazarı">
```

---

### keywords

```html
<meta name="keywords" content="HTML, CSS, JavaScript">
```

---

### http-equiv

```html
<meta http-equiv="refresh" content="5">
```

---

# 💡 Mantığı

`<meta>` etiketini şöyle düşünebilirim:

```text
HTML SAYFASI
│
├── Kullanıcıya gösterilen içerik
│   └── <body>
│
└── Sayfa hakkında bilgiler
    └── <head>
        └── <meta>
```

Örneğin:

```html
<meta charset="UTF-8">
```

→ Karakter kodlaması hakkında bilgi verir.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

→ Görüntüleme alanı ve başlangıç ölçeği hakkında bilgi verir.

```html
<meta name="description" content="HTML öğreniyorum.">
```

→ Sayfanın açıklamasını belirtir.

---

# 🧠 Meta Etiketini Parçalama

Şu örneğe bakalım:

```html
<meta name="description" content="HTML öğreniyorum.">
```

Bunu parçaladığımda:

```text
<meta
```

→ Meta etiketi

```text
name="description"
```

→ Meta bilgisinin adı/türü

```text
content="HTML öğreniyorum."
```

→ Bu bilginin değeri

```text
>
```

→ Etiketin bitişi

Yani temel mantık:

```html
<meta name="tür" content="değer">
```

---

# ⚠️ Dikkat Edilmesi Gerekenler

* `<meta>` genellikle `<head>` içerisinde kullanılır.
* `<meta>` doğrudan sayfada görünmez.
* `<meta>` kapanış etiketi almaz.
* `charset` karakter kodlamasını belirtir.
* `UTF-8` modern HTML belgelerinde yaygın olarak kullanılır.
* `viewport` özellikle responsive/mobil tasarım için önemlidir.
* `name` meta bilgisinin türünü belirtir.
* `content` meta bilgisinin değerini belirtir.
* `description`, sayfanın açıklamasını belirtmek için kullanılabilir.
* `keywords` günümüzde SEO açısından önemli bir araç değildir.
* Her `<meta>` etiketi SEO amacıyla kullanılmaz.

---

# ❌ Yaptığım Hatalar

* `<meta>` etiketini `<body>` içerisinde kullanmak.
* `<meta>` etiketinin ekranda görünen bir içerik oluşturduğunu düşünmek.
* `<meta>` etiketinin kapanış etiketi olduğunu düşünmek.
* `charset` ile `viewport`un aynı görevi yaptığını düşünmek.
* RGB gibi renk değerleriyle meta bilgilerinin ilişkili olduğunu düşünmek.
* `keywords` kullanmanın tek başına SEO sağlayacağını düşünmek.

---

# ✅ Doğru Kullanım

```html
<!DOCTYPE html>

<html lang="tr">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description" content="HTML öğrenme çalışma sayfam.">

    <meta name="author" content="Eyüp Arda">

    <title>HTML Meta Etiketleri</title>

</head>

<body>

    <h1>Meta Etiketleri</h1>

    <p>
        Bu sayfada HTML meta etiketlerini öğreniyorum.
    </p>

</body>

</html>
```

---

# 🧪 Bu Derste Yazdığım Örnekler

### Örnek 1 — Karakter kodlaması

```html
<meta charset="UTF-8">
```

---

### Örnek 2 — Mobil uyumluluk

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

### Örnek 3 — Sayfa açıklaması

```html
<meta name="description" content="HTML öğreniyorum.">
```

---

### Örnek 4 — Yazar

```html
<meta name="author" content="Eyüp Arda">
```

---

### Örnek 5 — Anahtar kelimeler

```html
<meta name="keywords" content="HTML, CSS, JavaScript">
```

---

### Örnek 6 — Refresh

```html
<meta http-equiv="refresh" content="5">
```

---

# 🧠 Kendime Notlar

> `<meta>` = Sayfa hakkında metadata verir.

> `<meta>` genellikle `<head>` içerisinde bulunur.

> `<meta>` ekranda doğrudan görünmez.

> `<meta>` kapanış etiketi almaz.

> `charset` = Karakter kodlaması.

> `UTF-8` = Yaygın kullanılan karakter kodlaması.

> `viewport` = Sayfanın görüntülendiği alanla ilgili ayarlar.

> `name` = Meta bilgisinin türü.

> `content` = Meta bilgisinin değeri.

> `description` = Sayfanın açıklaması.

> `author` = Sayfanın yazarı.

> `keywords` = Sayfayla ilişkili anahtar kelimeler.

> `http-equiv` = Bazı HTTP başlığı benzeri talimatları meta üzerinden belirtmek için kullanılabilir.

---

# 🔥 Bir Sonraki Hedef

**`<head>` bölümünü öğrenmeye devam etmek.**

Özellikle:

```html
<title>
<meta>
<link>
<style>
```

etiketlerinin görevlerini ve birbirlerinden farklarını öğrenmek.

Sonrasında CSS'ye geçerek HTML ile CSS'nin nasıl birlikte çalıştığını daha iyi anlamak.
