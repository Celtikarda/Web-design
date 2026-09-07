# 📚 Ders 9

## 🎯 Konu

CSS Gölgelendiriciler

---

## 📖 Öğrendiğim Kavramlar

- `box-shadow` = Kutulara gölge verir.
- `text-shadow` = Yazılara gölge verir.
- `inset` = `box-shadow` gölgesini kutunun içine verir.
- Blur = Gölgenin bulanıklık miktarını belirler.
- Blur değeri `0px` olabilir ve negatif olamaz.

---

## 📝 Sözdizimi

```css
box-shadow: yatay dikey bulanıklık renk;

text-shadow: yatay dikey bulanıklık renk;

box-shadow: inset yatay dikey bulanıklık renk;





💡 Mantığı
box-shadow bir HTML elementinin kutusuna gölge verir.
text-shadow ise elementin içindeki yazıya gölge verir.
Gölgenin konumu yatay ve dikey değerlerle belirlenir.
blur değeri gölgenin ne kadar bulanık olacağını belirler.
inset kullanıldığında gölge kutunun dışına değil, içine uygulanır.





⚠️ Dikkat
- box-shadow kutuya, text-shadow yazıya uygulanır.
- inset yalnızca box-shadow ile kullanılır.
- Blur değeri negatif olamaz.
- Blur için sabit bir maksimum değer yoktur.
- 0px blur kullanıldığında gölge keskin olur.
- Blur değeri arttıkça gölge daha geniş ve yumuşak görünür.





❌ Yaptığım Hatalar
- box-shadow ile text-shadow arasındaki farkı karıştırmak.
- inset özelliğinin ne işe yaradığını bilmemek.
- Blur değerinin maksimum bir değeri olduğunu düşünmek.





🧪 Örnekler
.kutu {
    box-shadow: 10px 10px 10px gray;
}
.yazi {
    text-shadow: 5px 5px 5px gray;
}
.kutu {
    box-shadow: inset 5px 5px 10px gray;
}
.kutu {
    box-shadow: 10px 10px 100px gray;
}





🧠 Kendime Not
box-shadow = Kutunun gölgesi
text-shadow = Yazının gölgesi
inset = Gölgeyi kutunun içine alır
Blur değeri arttıkça gölge daha bulanık olur.