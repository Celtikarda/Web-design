# 📚 Ders 18

## 🎯 Konu

HTML Formları ve Form Elemanları

---

## 📖 Öğrendiğim Kavramlar

* `<form>` kullanıcıdan bilgi almak için kullanılır.
* `<label>` input'un ne amaçla kullanıldığını belirtir.
* `<input>` kullanıcıdan veri almak için kullanılan temel form elemanıdır.
* `type` input'un türünü belirler.
* `text` normal yazı girişi sağlar.
* `password` şifre girişi sağlar.
* `email` e-posta girişi için kullanılır.
* `number` sayı girişi için kullanılır.
* `date` tarih seçmek için kullanılır.
* `checkbox` birden fazla seçim yapmak için kullanılır.
* `radio` aynı gruptan tek seçim yapmak için kullanılır.
* `<textarea>` birden fazla satırlık metin girişi sağlar.
* `file` dosya seçmek için kullanılır.
* `<button>` buton oluşturur.
* `submit` formu göndermek için kullanılır.
* `reset` formdaki girilmiş değerleri temizler.
* `required` alanın doldurulmasını zorunlu hale getirir.
* `<select>` açılır seçim listesi oluşturur.
* `<option>` select içerisindeki seçenekleri oluşturur.
* `id` elementi tanımlamak için kullanılır.
* `for` label ile ilgili input'u birbirine bağlar.
* `name` form verisinin adını belirtir.
* `value` form elemanının gönderilecek değerini belirtir.

---

## 📝 Sözdizimi (Syntax)

### Form

```html
<form>
    ...
</form>
```

### Input

```html
<input type="text">
```

### Label

```html
<label for="username">Kullanıcı adı:</label>
<input type="text" id="username">
```

### Password

```html
<input type="password">
```

### Email

```html
<input type="email">
```

### Number

```html
<input type="number">
```

### Date

```html
<input type="date">
```

### Checkbox

```html
<input type="checkbox">
```

### Radio

```html
<input type="radio">
```

### Textarea

```html
<textarea></textarea>
```

### File

```html
<input type="file">
```

### Button

```html
<button type="button">
    Buton
</button>
```

### Submit

```html
<button type="submit">
    Gönder
</button>
```

### Reset

```html
<button type="reset">
    Reset
</button>
```

### Required

```html
<input type="text" required>
```

### Select

```html
<select>
    <option>HTML</option>
    <option>CSS</option>
</select>
```

---

## 💡 Mantığı

Formları şu şekilde düşünebilirim:

```text
<form>
    ↓
Kullanıcıdan bilgi alacağım alan
    ↓
<input>
<textarea>
<select>
<button>
```

`input` etiketi farklı `type` değerleriyle farklı görevler üstlenebilir.

Örneğin:

```html
<input type="text">
```

→ Yazı

```html
<input type="password">
```

→ Şifre

```html
<input type="email">
```

→ E-posta

```html
<input type="number">
```

→ Sayı

```html
<input type="date">
```

→ Tarih

---

## 🏷️ Label Mantığı

`label` kullanırken `for` ile input'un `id` değerini eşleştirebilirim.

```html
<label for="username">
    Kullanıcı adı:
</label>

<input
    type="text"
    id="username"
>
```

Burada:

```text
label for="username"
        ↓
input id="username"
```

Birbirlerine bağlanırlar.

---

## ☑️ Checkbox ve Radio Farkı

### Checkbox

Birden fazla seçim yapılabilir.

```html
<input type="checkbox" name="language" value="html">
<input type="checkbox" name="language" value="css">
<input type="checkbox" name="language" value="javascript">
```

Örneğin kullanıcı:

```text
☑ HTML
☑ CSS
☐ JavaScript
```

şeklinde seçim yapabilir.

### Radio

Aynı `name` değerine sahip radio seçeneklerinden genellikle yalnızca biri seçilebilir.

```html
<input type="radio" name="gender" value="male">
<input type="radio" name="gender" value="female">
```

---

## 🔑 id, name ve value

Bunları birbirine karıştırmamalıyım.

```html
<input
    type="text"
    id="username"
    name="username"
    value="Eyüp"
>
```

### `id`

Elementi tanımlayan kimliktir.

### `name`

Form gönderildiğinde alanın adını belirtir.

### `value`

Alan tarafından taşınan değerdir.

### `for`

`label`ı ilgili input'un `id` değerine bağlar.

---

## ⚠️ Dikkat Edilmesi Gerekenler

* `<form>` form alanının genel yapısını oluşturur.
* `<input>` kapanış etiketi almaz.
* `<label>` ile input'u bağlamak için `for` ve `id` eşleştirilir.
* `radio` seçeneklerinin aynı grupta olması için `name` değerleri aynı olmalıdır.
* `checkbox` ile birden fazla seçim yapılabilir.
* `required` alanın zorunlu olmasını sağlar.
* `button` üzerinde `input` değil `type` kullanılır.
* `textarea` uzun metin içindir.
* `textarea` dosya seçmek için kullanılmaz.
* Dosya seçmek için `<input type="file">` kullanılır.
* `<select>` açılır listeyi, `<option>` ise listedeki seçenekleri oluşturur.

---

## ❌ Yaptığım Hatalar

### Hata 1

```html
<label for="password">
```

kullanıp input'a `id` vermemiştim.

### Doğrusu

```html
<label for="password">Şifre:</label>
<input type="password" id="password">
```

---

### Hata 2

```html
<button input="reset">
```

yazmıştım.

### Doğrusu

```html
<button type="reset">
```

---

### Hata 3

```html
<button input="submit">
```

yazmıştım.

### Doğrusu

```html
<button type="submit">
```

---

### Hata 4

`textarea` ile dosya seçmenin aynı şey olduğunu düşünmüştüm.

Doğrusu:

```html
<textarea></textarea>
```

→ Uzun metin

```html
<input type="file">
```

→ Dosya seçme

---

## ✅ Doğru Kullanım

```html
<form>

    <label for="email">
        E-posta:
    </label>

    <input
        type="email"
        id="email"
        name="email"
        required
    >

    <br>

    <button type="submit">
        Gönder
    </button>

    <button type="reset">
        Temizle
    </button>

</form>
```

---

## 🧪 Bu Derste Yazdığım Örnekler

* `<form>`
* `<label>`
* `<input>`
* `type="text"`
* `type="password"`
* `type="email"`
* `type="number"`
* `type="date"`
* `type="checkbox"`
* `type="radio"`
* `type="file"`
* `<textarea>`
* `<button>`
* `type="submit"`
* `type="reset"`
* `required`
* `<select>`
* `<option>`
* `id`
* `for`
* `name`
* `value`

---

## 🧠 Kendime Notlar

> `<form>` = Kullanıcıdan bilgi almak için form alanı.

> `<label>` = Input'un ne olduğunu belirtir.

> `for` = Label'ı input'un `id` değerine bağlar.

> `<input>` = Kullanıcıdan veri almak için kullanılır.

> `type` = Input'un görevini belirler.

> `checkbox` = Birden fazla seçim.

> `radio` = Aynı gruptan tek seçim.

> `<textarea>` = Uzun ve çok satırlı metin.

> `file` = Dosya seçme.

> `<select>` = Açılır liste.

> `<option>` = Açılır listenin seçeneği.

> `required` = Alan zorunlu.

> `submit` = Formu gönder.

> `reset` = Formu temizle.

> `id` = Elementin kimliği.

> `name` = Form verisinin adı.

> `value` = Form elemanının değeri.

---

## 🔥 Bir Sonraki Hedef

**HTML formlarını daha iyi anlamak ve `form`, `input`, `label`, `select`, `textarea` ve `button` etiketlerini kullanarak kendi başıma düzenli bir kullanıcı formu oluşturabilmek.**

Bir sonraki aşamada form elemanlarını **CSS ile düzenlemeye** başlayacağım.
