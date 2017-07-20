# Digital Signage Türkçe 


Digital Signage projesinin türkçe open source kodlarla yazılmış hali..

  - Kendine özgü editör!!
  - Slayt, resim, saat, video ve yazı elementleri
 


### Teknolojiler

Projede kullanılan temel teknolojiler:

* [interactJs] - Elementlerin sürükle bırak, boyutlandırma işlemleri ve daha fazlası!
* [Twitter Bootstrap] - Muhteşem arayüz tasarımı,
* [jQuery] - Bildiğiniz gibi :)

Ve tabiki de ücretsiz olarak paylaşmak için GitHub.

### Kullanımı

Herhangi bir kuruluma ihtiyaç yoktur.

"tasarim.html" sayfasını tarayıcınızda açmanız yeterlidir.
 
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

#### Yazı

*İlk olarak sol taraftaki menüden Mavi renkteki video elementi sürükle bırak yöntemiyle tasarım ekranına sürüklenir.
*Ekrana düşen dikdörtgen siyah çerçeveli elemente çift tıklanılır.
*Açılan editörde istenilen yazı yazılır ve kaydet butonuna tıklanılır.





> **Note:** "onizleme.html" sayfasında yer alan "youtubeUrlVideoUzunlugu()" fonksiyonunda key kısmına Google'dan youtube apisi için kendi key'inizi girmeyi unutmayın. [Youtube Api Key Alma](https://developers.google.com/youtube/v3/getting-started)  
```sh
  function youtubeUrlVideoUzunlugu(value) {
            var videosuresi=0;
            var durationstr;
            jQuery.ajax({
                url:"https://www.googleapis.com/youtube/v3/videos?id="+value+"&part=contentDetails&key=",
```



Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 80, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version}
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 80 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MOAR Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [interactJs]: <http://interactjs.io/>
   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
