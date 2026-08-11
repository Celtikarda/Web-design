## Çok Parametreli Fonksiyonlar

Bir fonksiyon birden fazla parametre alabilir.

```js
function alan(kısaKenar, uzunKenar) {
    return kısaKenar * uzunKenar;
}

document.write(alan(3, 12));
```

### Parametre ve Argüman

Fonksiyon tanımlanırken parantez içine yazılan değişkenlere **parametre** denir:

```js
function alan(kısaKenar, uzunKenar)
```

Fonksiyon çağrılırken parametrelere gönderilen değerlere **argüman** denir:

```js
alan(3, 12);
```

Burada:

```text
kısaKenar  ←  3
uzunKenar  ←  12
```

### `return` Kullanımı

`return`, fonksiyonun ürettiği değeri fonksiyonun çağrıldığı yere geri gönderir.

Doğru kullanım:

```js
return kısaKenar * uzunKenar;
```

`return` ifadesinden sonra geri döndürülecek değer yazılır.

```js
function alan(kısaKenar, uzunKenar) {
    return kısaKenar * uzunKenar;
}
```

`return` çalıştığı anda fonksiyon sona erer. Bu nedenle `return`'den sonra yazılan kod çalıştırılmaz:

```js
function test() {
    return 10;

    document.write("Bu çalışmaz.");
}
```

### Önemli

Parametreleri fonksiyonmuş gibi çağırmayız:

```js
alan(kısaKenar(3) * uzunKenar(12)); // Yanlış
```

Çünkü `kısaKenar` ve `uzunKenar` fonksiyon değil, **parametredir**.

Doğru kullanım:

```js
alan(3, 12);
```

**Kısaca:**

```text
Parametre → Fonksiyonun tanımında bulunur.
Argüman   → Fonksiyon çağrılırken gönderilen değerdir.
return    → Hesaplanan sonucu çağrıldığı yere geri gönderir.
```
