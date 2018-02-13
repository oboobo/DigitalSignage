# Digital Signage Türkçe 


Digital Signage projesinin türkçe open source kodlarla yazılmış hali..

  - Kendine özgü editör!!
  - Slayt, resim, saat, video ve yazı elementleri
  - Kısa bir süre için sadece 1920px 1080px olarak önizleme alınıyor.
  - Tasarım ekranı ise 960px 540px.


### Teknolojiler

Projede kullanılan temel teknolojiler:

* [interactJs] - Elementlerin sürükle bırak, boyutlandırma işlemleri ve daha fazlası!
* [Twitter Bootstrap] - Muhteşem arayüz tasarımı,
* [jQuery]

Ve tabiki de ücretsiz olarak paylaşmak için GitHub.

### Kullanımı


Bütün proje dosyalarını indiriniz.Ardından
"tasarim.html" sayfasını tarayıcınızda açmanız yeterlidir.
 
 Ancak Önizleme Yaparken eğer YouTube video url eklediyseniz, bunun için Api Key gereklidir.
 > **Note:** "onizleme.html" sayfasında yer alan "youtubeUrlVideoUzunlugu()" fonksiyonunda key kısmına Google'dan youtube apisi için kendi key'inizi girmeyi unutmayın. [Youtube Api Key Alma](https://developers.google.com/youtube/v3/getting-started)  
```sh
  function youtubeUrlVideoUzunlugu(value) {
            var videosuresi=0;
            var durationstr;
            jQuery.ajax({
                url:"https://www.googleapis.com/youtube/v3/videos?id="+value+"&part=contentDetails&key=",
```
 Tasarım sayfasını açtığınızda şöyle bir görüntü ekrana gelmektedir.
 ![Ana Ekran Görüntüsü](https://i.hizliresim.com/nWbD65.png)

#### Resim Elementenin eklenme işlemi adım adım

*İlk olarak sol taraftaki menüden yeşil renkteki resim elementi sürükle bırak yöntemiyle tasarım ekranına sürüklenir.
*Ekrana düşen dikdörtgen siyah çerçeveli elemente çift tıklanılır.
*Bilgisayardan resim seçilir ve kaydet butonuna tıklanılır.
*İstenilirse sürükle bırak yöntemiyle ekranda herhangi bir yere bırakılabilir veya yeniden boyutlandırılabilir.
![resimgif](http://i.picasion.com/pic86/18d02371c26b807b7a253dc86380de42.gif)

#### Arkaplan resminin eklenme işlemi adım adım

*Sağ taraftaki menüden tasarım ayarları butonuna tıklanılır.
*Açılan yerden bilgisayardan resim yüklenilerek arka plan resmi yüklenmiş olur.

![Arka Plan](http://i.picasion.com/pic86/4cd85b857ef70a38efc7bbe857b613c0.gif)


#### Saat Elementenin eklenme işlemi adım adım

*İlk olarak sol taraftaki menüden Mor renkteki saat elementi sürükle bırak yöntemiyle tasarım ekranına sürüklenir.
*Ekrana düşen dikdörtgen siyah çerçeveli elemente çift tıklanılır.
*İstenilirse özel ayarlar yapılabilir ve kaydet butonuna tıklanılır.

![Saatelementi](http://i.picasion.com/pic86/6f3d8e3ae93305c55f82e0186792c612.gif)

## Önizleme

Resim, saat ve arkaplan işlemlerinden sonra oluşan önizleme

![Önizleme](https://i.hizliresim.com/9dYz2o.png)

### Diğer Elementlerin Kullanımı


#### Video

*İlk olarak sol taraftaki menüden Sarı renkteki video elementi sürükle bırak yöntemiyle tasarım ekranına sürüklenir.
*Ekrana düşen dikdörtgen siyah çerçeveli elemente çift tıklanılır.
*Açılan ekranda youtube URL girilir istenilirse o anda önizleme yapılır ve kaydet butonuna tıklanılır.

![Youtube](http://i.picasion.com/pic86/c04fedcadbba2f2d20ded30673f590ad.gif)

> **Note:** "onizleme.html" sayfasında yer alan "youtubeUrlVideoUzunlugu()" fonksiyonunda key kısmına Google'dan youtube apisi için kendi key'inizi girmeyi unutmayın. [Youtube Api Key Alma](https://developers.google.com/youtube/v3/getting-started)  
```sh
  function youtubeUrlVideoUzunlugu(value) {
            var videosuresi=0;
            var durationstr;
            jQuery.ajax({
                url:"https://www.googleapis.com/youtube/v3/videos?id="+value+"&part=contentDetails&key=",
```
#### Yazı

*İlk olarak sol taraftaki menüden Mavi renkteki yazı elementi sürükle bırak yöntemiyle tasarım ekranına sürüklenir.
*Ekrana düşen dikdörtgen siyah çerçeveli elemente çift tıklanılır.
*Açılan editörde istenilen yazı yazılır ve kaydet butonuna tıklanılır.
![yazı](http://i.picasion.com/pic86/dc913edacf550f0f83824cc6aa2b30b1.gif)

#### Slayt

*İlk olarak sol taraftaki menüden kırmızı renkteki slayt elementi sürükle bırak yöntemiyle tasarım ekranına sürüklenir.
*Ekrana düşen dikdörtgen siyah çerçeveli elemente çift tıklanılır.
*Açılan ekranda sağ taraftan slaytın içeriğine eklenilecek olan elementler seçilir.
*Video,resim, yazı farklı elementleride bir arada kullanabilirsiniz. 
*Geçiş süreleri ayarlanır. Video için, YouTube'dan apisinden çekilen video süresi otomatik verilir. Bunun için önizleme sayfasında yukarıda video elementi için belirtilen YouTube Key'i girmeyi unutmayınız.

![Slayt](http://i.picasion.com/pic86/fb2736e1e0d26acb2df3a860b2e1fd8a.gif)










   [interactJs]: <http://interactjs.io/>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
