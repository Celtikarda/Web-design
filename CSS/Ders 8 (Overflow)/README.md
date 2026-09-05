# 📚 Ders 8

## 🎯 Konu

CSS `overflow` özelliği

---

## 📖 Öğrendiğim Kavramlar

- `overflow` = Taşma
- `overflow: hidden` = Taşan içeriği gizler
- `overflow: scroll` = Her zaman kaydırma çubuğu gösterir
- `overflow: auto` = Gerektiğinde kaydırma çubuğu gösterir
- `overflow: visible` = Taşan içeriği göstermeye devam eder

---

## 📝 Sözdizimi

```css
overflow: hidden;
overflow: scroll;
overflow: auto;
overflow: visible;





💡 Mantığı
Bir kutunun genişliği veya yüksekliği içindeki içerik için yeterli olmadığında içerik kutunun dışına taşabilir.
overflow özelliği, kutudan taşan içeriğin nasıl davranacağını belirler.





⚠️ Dikkat
- overflow varsayılan olarak visible değerindedir.
- hidden kullanıldığında taşan içerik görünmez.
- scroll kullanıldığında içerik taşmasa bile kaydırma çubuğu gösterilebilir.
- auto yalnızca gerektiğinde kaydırma çubuğu oluşturur.




❌ Yaptığım Hatalar
- overflow değerlerinin ne işe yaradığını karıştırmak
- auto ile scroll arasındaki farkı karıştırmak





🧪 Örnekler
#buyuk {
    width: 30px;
    height: 30px;
    background-color: lightblue;
    overflow: auto;
}