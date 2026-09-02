📚 Ders 4
🎯 Konu
Border özellikleri
📖 Öğrendiğim Kavramlar
- border-style = Kenarlığın stilini belirler.
- border-width = Kenarlığın kalınlığını belirler.
- border-color = Kenarlığın rengini belirler.
- border = Border özelliklerini kısa şekilde yazmamızı sağlar.
- border-radius = Kutunun köşelerini yuvarlatır.
- groove = Kenarlıkta ışık-gölge etkisi oluşturarak oyulmuş/oluklu bir görünüm verir.
- solid = Düz kenarlık oluşturur.
- dotted = Noktalı kenarlık oluşturur.
- dashed = Kesikli kenarlık oluşturur.
- double = Çift çizgili kenarlık oluşturur.
📝 Sözdizimi
border: kalınlık stil renk;

border-width: 3px;
border-style: solid;
border-color: black;

border-radius: 10px;

💡 Mantığı
border bir elementin çevresine kenarlık eklememizi sağlar.
Örneğin:
border: 3px groove black;

Burada:
- 3px → kenarlığın kalınlığı
- groove → kenarlığın stili
- black → kenarlığın rengi
border-radius ise kutunun köşelerini yuvarlatır.
Birden fazla değer verirsek kenarları ayrı ayrı kontrol edebiliriz:
border-style: double dashed dotted solid;

Sıralama:
üst → sağ → alt → sol
⚠️ Dikkat
- border: 3px; tek başına istediğim border görünümünü oluşturmaz; border stilinin de belirlenmesi gerekir.
- border kısa yazımı, diğer border özelliklerinin üzerine yazabilir.
- border-radius değerlerinin sırası önemlidir.
- Dört değer kullanırken sıra üst, sağ, alt, sol şeklindedir.
- groove gibi 3D border stillerinin görünümü border kalınlığına göre değişebilir.
❌ Yaptığım Hatalar
- border-style: dotted; yazdıktan sonra border: 3px; kullanarak önceki border ayarını ezdim.
- border kısa yazımının sadece kalınlık değil, stil ve renk ile birlikte kullanılabileceğini öğrendim.
🧪 Örnekler
h1 {
    border-style: solid;
    border-color: aqua;
    border-radius: 0px 0px 10px 10px;
}

h2 {
    border: 3px groove black;
    border-radius: 10px 10px 0px 0px;
}
p {
    border-width: thin;
    border-style: double dashed dotted solid;
}
🧠 Kendime Not
Border = kalınlık + stil + renk
border: 3px solid black;
Ayrıca border-radius kutunun köşelerini yuvarlatır.
4 değer kullanırsam: üst → sağ → alt → sol.