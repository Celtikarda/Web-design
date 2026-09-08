Gün 1 --> Terminal, klasör ve dosya işlemleri.

pwd
Açılım="Power Working Directory"
Akılda kalıcı olması için: Çalışan dizinin yolunu "print" et.
Anlaşılması için output şöyle olmalı:
──(kali㉿kali)-[~/Desktop]
└─$ pwd
/home/kali/Desktop


whoami
Açılımı="Who am ı"
Akılda kalıcı olması için: Zaten türkçeye çevirmek sonucu getiriyor. "Ben kimim?" sorusu bilgisayarı hangi kullanıcı kullanıyor sorusunun cevabıdır.
Anlaşılması için output şöyle olmalı:
┌──(kali㉿kali)-[~/Desktop]
└─$ whoami
kali


ls
Açılımı="List"
Akılda kalması için : Bulunduğumuz klasörün içindeki dosyaları "listeler".
Anlaşılması için output şöyle olmalı:
┌──(kali㉿kali)-[~/Desktop]
└─$ ls    
Arda  BosDosya 
Mesela burda Masaüstündeki dosyalar gözüktü.
 

cd
Açılımı="Change directory"
Tanım= Bulunduğumuz dizinden başka dizine geçmek için kullanılır. "cd klasörIsmi" şeklinde kullanılır.
Akılda kalıcı olması için: Terminaldeki bulunduğumuz dizini "değiştirmek=change" için kullanılır.
Anlaşılması için output şöyle olmalı:
┌──(kali㉿kali)-[~/Desktop]
└─$ cd        
                                                                             
┌──(kali㉿kali)-[~]
└─$ cd // ile ilk klasöre yani işletim sisteminin kurulduğu yere geldik.

Mesela başka dizine geçmek için cd dizinIsmi şeklinde yazılabilir.
Anlaşılması için output şöyle olmalı:
──(kali㉿kali)-[~]
└─$ cd Desktop
                                                                             
┌──(kali㉿kali)-[~/Desktop]
└─$ // Görüldüğü üzere "cd Desktop" ile masaüstüne ayak basmış olduk.


mkdir
Açılımı= "Make Directory"
Tanım= Yeni klasör oluşturmak için kullanılır. "mkdir klasörIsmi" şeklinde kullanılır.
Akılda kalıcı olması için: Açılımı bilindiğinde çok kolaydır. "mk" make olarak akılda tutulmalı.
Anlaşılması için output şöyle olmalı:
┌──(kali㉿kali)-[~/Desktop]
└─$ cd Desktop   // "cd Desktop" ile masaüstüne geldik. Oluşturacağımız klasörü bu sayede masaüstüne atacak.
                                                                             
┌──(kali㉿kali)-[~/Desktop]
└─$ mkdir ornekKlasör  // "mkdir klasörIsmi" dedik ve klasörümüz oluşturduk.
                                                                             
┌──(kali㉿kali)-[~/Desktop]
└─$    // Sonra tekrardan masaüstündeyiz diye bize gösterir. 


touch
Açılım yoktur direkt kendisidir: "touch"
Tanım= Yeni ve boş bir dosya oluşturmak için oluşturulur.
Akılda kalması için= Boş dosya oluşturmak için kullanılır. Tuttuğun elin (touch) boş (Boş dosya) olmasından aklına gelsin.
Anlaşılması için output şöyle olmalı:
┌──(kali㉿kali)-[~]
└─$ cd Desktop // "cd Desktop" ile masaüstüne geldik.
                                                                             
┌──(kali㉿kali)-[~/Desktop]
└─$ cd Arda   // Masaüstünde bulunan "Arda" adlı klasöre "cd Arda" yardımıyla ulaştık.
                                                                             
┌──(kali㉿kali)-[~/Desktop/Arda]
└─$ touch ornekMetin.txt // "Arda" adlı klasörün içine touch ile "ornekMetin.txt" adlı metin dosyasını oluşturduk.


ls -la
Açılım: "list long listing all"
Tanım= Ayrıntılı bir şekilde klasörleri listelemeye yarar.
Akılda kalması için= Klasörün secretları ortaya çıkıyor.
Anlaşılması için output şöyle olmalı:
┌──(kali㉿kali)-[~/Desktop/Arda]
└─$ cd // "cd" ile default konuma geldik.
                                                                             
┌──(kali㉿kali)-[~]
└─$ cd Desktop // Masaüstüne geldik.
                                                                             
┌──(kali㉿kali)-[~/Desktop]
└─$ ls -al  // Bu komutla beraber masaüstünde bulunan bütün gizli ve gizli olmayan dosyaları görebiliriz.
total 16
drwxr-xr-x  4 kali kali 4096 Sep  8 11:18 .
drwx------ 18 kali kali 4096 Sep  8 11:26 ..
drwxrwxr-x  4 kali kali 4096 Sep  8 11:28 Arda
-rw-rw-r--  1 kali kali    0 Sep  8 10:34 BosDosya
drwxrwxr-x  2 kali kali 4096 Sep  8 11:18 ornekKlasör


