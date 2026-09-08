Edabit sana zaten array'i fonksiyona verecek:
getFirstValue([1, 2, 3])
Burada:
index:     0   1   2
           ↓
array:    [1,  2,  3]
İlk elemanın index'i 0 olduğu için:
function getFirstValue(arr) {
    return arr[0];
}
Senin için önemli olan kısım
Şunu:
arr[0]
şöyle oku:
arr dizisinin 0. indexindeki eleman

Örneğin:
let sayilar = [80, 5, 100];

console.log(sayilar[0]);
Sonuç:
80