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

## %PAGE
Her çıktı bizim için bir sayfadır.
Daha sonra default da page bir diye sayfa default olarak gelir.
* Genel Özellikler : Birden fazla sayfa üzerinde işlem yapılacaksa sayfa sayacı ile nasıl numaralanması gerektiği seçilir.
* Çıktı Seçenekleri: Sayfanın dikey mi yatay mı olduğu bu kısımdan seçilir.
* Artan Ekran: 

![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/7fff1368-4d4d-40b9-a1ae-5894f738bc91)
%PAGE1 altında default olarak Main daha çok tabloların basıldığı yerdir. Eğer tablodaki veriler main içerisine sığmaz ise ikinci sayfaya geçmesini sağlar. Sayfa yapısının kontrolü için kullanılmaktadır.

## Pencere
Pencere oluşturmak için %PAGE kısmına sağ tıkladığımız zaman ,yarat , kes , kopyala , yapıştır  , sil ,genişlet ,sıkılıştır  kısımlardan oluşmaktadır. Genişlet kısmı page altındaki tüm içerikleri görmek istersek seçilir. Sıkıştır ise page altında bulunan içerikleri görmek istemezsek kullanılır.
Pencere oluştururken %page sağ tıkla , yarat ,pencere , sırasıyla işlemlerini gerçekleşince oluşur.
Penceremiz bağlığı içerdiği için header ismi verilir. Oluşturduğumuz pencerelerin özellikleri aşağıdaki şekildedir.
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/520f105c-39fe-43bc-9cff-d1033235e39c)
* Pencere genel özellikler , çıktı seçenekleri , koşullar dan oluşmaktadır.Genel özellikler: pencere tipi ana pencere default olarak gelen ( main ) kısmı gösterir.Biz bu kısım da ikinci pencere seçilir. İkinci pencere ,verileri sonraki sayfaya genişletmez .Belirtildiği  sayfa yeterli  alan varsa tam metni yazdıracaktır.
* Çıktı Seçenekleri: Bu penceremizin konumu sağ taraftan hareket ettirebiliriz  yada çıktı seçeneklerinden genişlik , yükseklik , sol kenarlık , sağ kenarlık  , çizgi , gölgelendirme , işlemleri  bu kısımda ayarlanır.
* Koşullar: Birden fazla sayfamız bulunuyor ise bu pencerenin hangi sayfada ve hangi mantıkla görüneceğini belirlenir.

## Metin 
Pencere ekranına metin eklemek ve çıktıda görünmesini istediğimiz içerikler bu kısım da yazılır.
Oluşturduğumuz pencereye sağ tıklayarak yarat metin ile oluşturulur .Birden fazla metin oluşturursak alt alta  bu metinleri yazar.

## Sayfa Numarası
Sayfa numarası eklemek istersek pencereden bir metin oluşturulur ve sayfanın alt kısmına konulur.
Sayfa numarası sabit değil yani bunu bir metin olarak ekleyemeyiz(sayfa numarası dinamik olarak yeni sayfa eklendiğinde değişebilmelidir.) .O yüzden de değişken olarak tanımlanır.
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/b0e7d1a3-95aa-4cb2-9016-96cad948bdaa)

Artı işaretine tıklayıp && arasına değişkenimizin ismi yazılır. Sayfa numarasını tutması için sfsy-page yazalım.
Yazdığımız bu değişkende değişiklik yapmak istersek de + işaretin yanındaki kalemden değişiklik yapılabilir.

## Şablon
Verilerin belli hizada görünmesi sağlanır. Biz bu kısma birden fazla içeriği hizalı bir şekilde yazmak istediğimiz için de her bir içerik de metin oluşturulur  şablon kullanılmaz ise hizalı bir şekilde görünebilmesi için space dikkat edilerek tekrar tekrar uğraşmamız gerekmektedir .Bunun yerine şablon oluşturursak yazdığımız içerikleri belirlediğimiz ölçülere göre düzenini kendi oluşturur.


Bunun için de pencereye sağ tıklayarak şablon oluşturabiliriz.
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/cda38a7f-ea35-40ec-808c-679a1ce40352)
Yukarıdaki ekran da ayrıntılar kısmına tıklayalım.
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/e56b6bde-235b-45f4-9117-c076d63eac66)
Son kısmı  kaç tane satırdan oluşacağını gösterir. Yükseklik her bir satır arasında ki mesafeyi gösterir .Kaç adet sütunum olmasını istiyorsak da 1. cm cinsinden büyüklüğü şeklinde her sütun için genişlik belirlenir. Yaptığımız içerik te her bir sütun için belirlediğimiz büyüklük toplamı yukarıdaki genişliğin toplamı kısmına yazılmalıdır.
Bu şablonun bağlı olduğu pencerenin genişliği sütun için belirlenen değerden büyük veya eşit olmalıdır ki içerisine sığabilmesi için gereklidir.

## Tabloyu Smartform İle Ekranda Görünmesi 
Oluşturacağımız tabloyu kendi oluşturduğumuz pencerelerin altına da tablo oluşturularak da  yapılır ama o zaman tablo bir sayfaya sığmayınca (taşınca) diğer sayfaya geçmez .O yüzden de tablo sayfaya sığmadığı zaman diğer sayfaya geçebilmesi için smartform oluşturduğumuz da default olarak gelen main ana penceresinin altına tablo eklenir.
Tablo oluşturulunca  başlık alanı , ana alan ,  sayfa altlığı olarak  üç olandan oluşur .İlk olarak tablomuzdan ayrıntılara gidelim.

![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/bfa2ca89-ac21-4cbb-9593-ddfa60ea2fcc)
Bu kısımda LTYPE1 default olarak gelir. Burada kaç sütun ve her sütun ne kadar genişlikte olduğu belirlenir.
Sütun genişliklerinin toplamı da tablo genişliği kısmına verilir. Main genişliği tablonun genişliğinden büyük veya eşit olması gerekmektedir.

LTYPE2 kısmı tablonun en altına yeni bir alan oluşturmak için kullanılmıştır.LTYPE1 de dört sütundan oluşmaktadır ama LTYPE2 ise 3 sütundan oluşur .Burada önemli olan sütun değil de toplam genişlik  göre istenilen sayıda sütun oluşturulabilir.

Daha sonra başlık altına sağ tıklayarak yarat tablo satırı oluşturulur. Oluşan satırdan satır tipi seçilir biz ilk olarak LTYPE1 seçeriz .Bu içeriği seçtikten sonra seçilen içerik de ne kadar sütun varsa o kadar alan ekler. Bizim dört tane sütunumuz olduğun için dört adet ekler.
Oluşan her bir alan altına metin oluşturulur. Oluşturulan bu metin kısımlarına da sütun da hangi ismin görünmesini istiyorsak onun ismi yazılır.![image]
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/8bdb5cfc-a3a5-4dab-9357-3c99d8eb862c)

Tabloyu ana alanın altında yarat tablo satırı oluştur .Daha sonra da satır t
ipi olarak da LTYPE1 seçilir.


Ana alan kısmına tablo yazacağımız için ilk olarak bu kullanacağımız internal tablo structure ve table type tanımlamamız gerekmektedir. Genel tanımlamalar kısmına  genel veriler ile (Global tanımlama) structure , internal tablomuzu  ve tablonun altına bir satır ekleyip  o satırda aradığımız içerikten kaç tane olduğunu görmek için integer bir değişken tanımlanır.
Internal tablo oluşturmak için type table of olması gerekmektedir. Ama bu kısım da type ve type ref to olduğu için internal tabloyu direk bu kısım da oluşturamayız. O yüzden de istersek se11 den table type oluşturabiliriz yada tipler kısmın da  table type scarr dan oluşturabiliriz. Oluşturduğumuz bu table type  tipinde internal tablomuzu oluşturabiliriz.
![image](https://github.com/sumeyyaakbulut/Smart-Forms/assets/62395974/68a6f6db-1833-4464-8e44-c3daf2520d69)








