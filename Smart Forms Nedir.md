# Smart Forms Nedir

* Smart Formlar ile form yazdırılır .Yazdırılan formlar internet E-posta , yazıcı, faks makinesine gönderilmesi sağlanır.
* Müşteri ilişkileri yönetim(CRM) , SD ,HR ,ERP  gibi modüllerde formlar kullanılır.Bu sayede formlar tasarlanıp yazdırılır.
* Smart form ile basit grafik araçları ile formları değiştirebiliriz .Metinler ,resimler  ve barkodlar gibi içerikleri smart form gömebiliriz.
* SAP de çıktı alan tasarım olarak smart form ve adobe formlar kullanılabilir.
* Smart Forms ile veriler statik ve dinamik tablolardan alınabilir. Tablo başlığı alt toplam ile tetiklenen  olaylar tarafından belirlenir ve  veriler sonuçtan önce sıralanmış olur.
* Stil vermek istersek de Smarttyles kullanılır.

## Form Niteliği

Smartforms tcode yazılır, form isim verilir.Sol tarafta genel yapının olduğu kısımdır, orta kısım sol daki  tıkladığımız içeriğin detayını görüntülediğimiz kısımdır. Sağ tarafta ise teknik tasarımın anlık olarak görünmesi sağlanır.Form Niteliği , kimin ne zaman oluşturduğu veya değiştirdiği ile ilgili bilgileri tutar.Genel özellikleri gibi çıktı seçeneklerinden sayfa biçimi seçilir default olarak DINA4 (A4)  ekranı gelir. Biz istediğimiz ekranı boyutunu bu kısımdan seçebiliriz.
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/4493c891-2715-45de-a91f-cbcf3adc770c)


## Form Arayüzü

Form arayüzü dört başlıktan oluşmaktadır .İçe aktar , dışa aktar  , tablolar , istisnalar dan oluşmaktadır.
Programdan smartform çağıracağımız için smartform fonksiyona benzetilebilir.
* İçe aktar: smart form dışarıdan göndereceğimiz parametrelerdir .Ekranda görülen default standart olarak tanımladıkları  zorunlu alanlar bulunmaktadır.
* Dışa aktar: kısmı ise smart form çağırdığımız  kısımda ki  data  döneceği yapılardır.Tablolar:İstisnalar:
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/110706c2-672e-4431-a4b6-3f530cafdf21)


## Genel Tanımlar
Genel veriler, tipler , alan sembolü , başlangıç durumu , form rutinleri , miktar alanlarından oluşmaktadır.
* Genel verilerde: data tanımlamak için oluşturduğumuz include da , globalde data tanımlaması şeklindedir.
* Tipler: local type tanımlamak istersek kullanılır.
* Başlangıç durumunu getir:  ise  çıktı açılır açılmaz görüntülenen kısımdır initialization.
* Giriş Parametreleri program satırında kullanacağımız parametreler bu kısımla tanımlanır

![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/a5b6fb9e-050a-4963-8c9a-ce35bc2bc947)





