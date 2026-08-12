## Fonksiyon İçerisinde `for` Döngüsü

Bir fonksiyonun içinde `for` döngüsü kullanılabilir. Fonksiyona gönderilen parametre, döngünün kaç kere çalışacağını belirleyebilir.

```js
function sıfırdan(x) {
    for (let n = 0; n <= x; n++) {
        document.write("Merhaba<br>");
    }
}

let x = Number(prompt("X:"));
sıfırdan(x);
```

Örneğin `x = 5` girilirse döngü:

```text
0 → 1 → 2 → 3 → 4 → 5
```

olacak şekilde **6 kez** çalışır.

### `for` Döngüsünde Önemli Nokta

`for` ifadesinin sonunda yanlışlıkla `;` koyarsak döngünün gövdesi boş kalır:

```js
for (let n = 0; n <= x; n++); // Yanlış
{
    document.write("Merhaba");
}
```

Buradaki `;`, `for` döngüsünü bitirir. `{ }` bloğu artık döngünün gövdesi değildir.

Doğru kullanım:

```js
for (let n = 0; n <= x; n++) {
    document.write("Merhaba");
}
```

### Mantık

```text
Fonksiyon
   ↓
Parametre (x)
   ↓
for döngüsü
   ↓
0'dan x'e kadar tekrar
   ↓
Her turda işlem
```

**Not:** `i++` veya `n++`, döngünün her tur sonunda değişkeni 1 artırmasını sağlar.
