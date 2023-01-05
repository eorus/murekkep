---
title: WordPress Kurulum Sonrası Ayarlar Rehberi
author: Alper
type: post
date: 2011-01-24T20:13:29+00:00
url: /wordpress-kurulum-sonrasi-ayarlar-rehberi/
dsq_thread_id:
  - 949294194
categories:
  - Teknoloji
tags:
  - tema
  - wordpress

---
**WordPress kurulumu** belirtildiği gibi gerçekten 5 dakika gibi kısa bir zamana sığdırılabiliyor. WordPress kurulan her blogun yapısı muhtemelen farklıdır. Ancak genel ayarlar tabir edebileceğimiz düzenlemeleri, her yeni **wordpress kurulumu** sonrası aynı işleri belirli bir sırada yaptığımızı düşünürsek, **wordpress kurulum sonrası ayarları** listeleyebiliriz.

WordPress blogunun ilk aşamasında veritabanı oluşturdunuz ve wordpress kurulumunu gerçekleştirdiniz. Hemen ardından sırayla yapılması gerekenler listesini belirlemeye çalışacağız. Bu liste içerisinde elbette sıralama her wordpress kullanıcısına göre değişiklik gösterecektir. Eklemek ya da düzeltmek istediklerinizi yorumlarınızda belirtebilirsiniz.

## WordPress Kurulum Sonrası Ayarlar Rehberi

### Kalıcı Bağlantıları Değiştirme

WordPress kurulumunu gerçekleştirdiğinizde ve yeni oluşturduğunuz bloga baktığınızda ilk gözünüze çarpan kısım tarayıcı adresindeki kalıcı bağlantı URL&#8217;si olacaktır. Varsayılan olarak **http://site.com/?p=123** gibi gelen yazı adresini **http://site.com/yazı-adresi** şeklinde veya alternatif kalıcı bağlantılarla wordpress içerisinden değiştirebiliyorsunuz. WordPress admin paneli üzerinden **Ayarlar > Kalıcı Bağlantılar** ile ilgili ekrana ulaşabilirsiniz.

Önceliği kalıcı bağlantıları değiştirme kısmına vermemiz **SEO** açısından da iyi olacaktır. Çünkü yazdığınız her yazının arama motorları tarafından bu şekilde indeksleneceğini düşünürseniz daha sonra kalıcı bağlantılarda yapacağınız bir değişiklik, arama motorlarının indekslediği sayfaların **404 hatası** vermesine yol açacaktır. Bu yüzden ilk değişikliği kalıcı bağlantılarda yapıyoruz.

Bunun yanısıra wordpress altyapısında yazıları eklediğiniz **kategoriler** ve yazılara eklediğiniz **etiketlerin** kalıcı bağlantı isimlerini de buradan belirleyebilirsiniz.

Bkz. Using_Permalinks

### Admin Kullanıcısı ve Yazarlar

Güvenlik sebebiyle **wordpress kurulumu** sırasında oluşan &#8220;**admin**&#8221; kullancısını sistemden siliyoruz. Bu sırada aynı ekrandan **blog yazarı** olarak **yönetici** haklarıyla kendi kullanıcımızı ekliyoruz. WordPress yönetim panelinden yeni kullanıcı oluşturmak için **Kullanıcılar > Yeni Ekle** ya da **admin kullanıcısını silmek** için **Kullanıcılar > Kullanıcılar** şeklinde ulaşabilirsiniz. Yeni oluşturacağınız kullanıcı profilini mutlaka yönetici haklarıyla oluşturmanız gerektiğini hatırlatalım.

### Genel Ayarlar, Yazma, Okuma, Tartışma

WordPress yönetim panelinde ayarlar sekmesine geldiğinizde wordpress ile gelen genel, okuma, yazma ve tartışma ayarlarına göz atmak ve istediğiniz şekilde bu ayarları belirlemekte fayda var. Çünkü bir müddet sonra bu bölgeye bir daha uğramıyorsunuz ve en başta belirlediğiniz ayarlar siz bir daha bakana kadar burada kalıyor.

**Genel Ayarlar** : Site Başlığı, saat ve tarih ayarları, yönetici eposta adresi gibi genel ayarların bulunduğu kısım.  
**Yazma** : Yazı ve bağlantı kategorilerinin varsayılanlarının belirlenmesi, uzaktan ve eposta ile blog yazma ayarlarının bulunduğu kısım.  
**Okuma** : Yazıların ön sayfa görünümlerinin belirlenmesi, beslemelerde ve ana sayfada görünüm şekli ile karakter kodlaması ayarlarının bulunduğu kısım.  
**Tartışma** : Tüm yorum ve yorumların gösterimine ilişkin ayarların tutulduğu kısım.

### Feedburner Hesabı Oluşturun

WordPress ile blog oluşturduysanız ve hala bir **feedburner** hesabınız yoksa mutlaka bir tane edinin. <a href="http://feedburner.google.com/" target="_blank">Feedburner</a> sadece istatistik anlamında RSS izleyicilerinin, takipçilerinin datalarını tutmakla kalmayıp aynı zamanda sitenizin beslemelerini en iyi şekilde takip etmenize olanak sağlar. Bir google hesabınız varsa feedburner üzerinden giriş yapıp hızlı bir şekilde wordpress blogunuzun rss adresini feedburner ile takip edebilirsiniz.

### WordPress Temanızı Yükleyin ve Aktifleştirin

Belki de tüm wordpress kurulum işleminden önce hazır edilmesi gereken maddelerden bir tanesi wordpress temasını belirlemek. Binlerce **ücretsiz wordpress teması** arasından zevkinize ya da sitenizin içeriğine uygun bir tane seçmek zor olabiliyor. Eğer wordpress blogunuz için bir tema seçtiyseniz bu aşamada temayı **Görünüm > Temalar > Yükle** kısmından temayı yükleyebilir ve akabinde aktifleştirebilirsiniz.

### Google Analytics Kullanın

WordPress kurulumu sonrası bayağı bir yol aldınız. WordPress temasını kurup aktifleştirdiniz. Bu aşamada unutmadan **google analytics javascript kodunu** ilgili temaya eklemeniz gerekiyor. Şu anda web üzerindeki en iyi istatistik takip servisi olan [Google Analytics][1] ile sitenize gelen ziyaretçilerin **demografik bilgileri**, sitenizin görüntüleme sayısı gibi olabilecek her türlü **istatistik** verisini Google Analytics ile gözlemleyebilir ve sitenizin istatistiklerini takip edebilirsiniz.

**Google Analytics** kodunu manuel olarak yerleştirmede sıkıntı yaşarsanız <a href="http://wordpress.org/extend/plugins/google-analytics-for-wordpress/" target="_blank">Google Analytics for WordPress</a> eklentisi ile kolayca bu işlemi gerçekleştirebilirsiniz.

### Hakkında Sayfasını Oluşturun

En çok geçiştirilen ve genelde kısa tutulan bir sayfa olan hakkında sayfasını mutlaka hazırlayın. Yazılarınızı yazmaya başladıktan sonra ziyaretçileriniz sitenizi takip etmeye başladıkça sitenizin hakkında sayfasına bakıp bilgi almak isteyeceklerdir. İyi bir **hakkında sayfası** ile ziyaretçilerinize sitenizin yapısı ve genel olarak kendiniz hakkında kısa bilgiler aktarabilirsiniz.

WordPress yönetim panelinde **Sayfalar > About** şeklinde hazır gelen hakkında sayfasını düzenleyip oluşturabilirsiniz.

### Olmazsa Olmaz WordPress Eklentileri

WordPress blog platformunun en güzel özelliklerinden birisi şüphesiz hayatı kolaylaştıran **wordpress eklenti dizini**. Özellikle wordpress 2.7 sonrası otomatik olarak kurulup, kaldırılabilen ve güncelleştirilebilen wordpress eklentilerini kolayca yönetebilmekteyiz. **WordPress kurulumu** tamamlanıp yukarıdaki adımları sırasıyla hayata geçirdikten sonra olmazsa olmaz diyebileceğimiz wordpress eklentilerini kurabiliriz.

Bir wordpress kurulumu sonrası kurulması ve etkinleştirilmesi gereken eklentilerin kısa bir listesi aşağıdaki gibidir. Bunların dışında sizin önemli gördüğünüz ve kullandığınız **wordpress eklentileri** varsa ayrıca yorumlarınızda belirtebilirsiniz.

&#8211; <a href="http://akismet.com/" target="_blank">Akismet</a> : WordPress geliştiricilerinden spam kontrolü ve yönetimi için wordpress eklentisi.  
&#8211; <a href="http://wordpress.org/extend/plugins/all-in-one-seo-pack/" target="_blank">All in one SEO Pack</a> : WordPress blogunuz için başlık, anahtar kelime ve tanımları belirleyebilir. WordPress temasından bağımsız şekilde SEO için önemli olan başlıkları otomatik ekleyebilirsiniz.  
&#8211; <a href="http://wordpress.org/extend/plugins/google-analytics-for-wordpress/" target="_blank">Google Analytics for WordPress</a> : Yukarıda da bahsettimiz gibi google analytics javascript kodunu tema bağımsız kolayca eklemenizi sağlayan eklenti.  
&#8211; <a href="http://wordpress.org/extend/plugins/wp-super-cache/" target="_blank">WP Super Cache</a> : WordPress kurulumunu yeni bir blog için yaptıysanız muhtemelen ilk başlarda kullanmanızın gerekmediği bir wordpress eklentisi WP Super Cache.  
&#8211; <a href="http://wordpress.org/extend/plugins/google-sitemap-generator/" target="_blank">Google XML Sitemaps</a> : WordPress blogunuz için xml site haritası oluşturan **Google XML Sitemaps** eklentisi için ayarlarının nasıl olması gerektiğini araştırabilirsiniz ancak olduğu gibi bırakırsanız ekstra bir ayara gerek duymadan wordpress blogunuzda yaptığınız değişiklikler, yeni yazı gönderiminde otomatik olarak arama motorlarını uyaran bir yapıya sahiptir.

Temel olarak bir wordpress kurulumu sonrası sırasıyla yapılması gerekenler belirli eklentilerle beraber bunlar gözüküyor. Bir checklist gibi sırasıyla uygulanabilir liste içerisinde kendinize göre öncelik sıranız değişiklik gösterecektir. Belirli bir kurulum sonrası planı olmayanlar için faydalı olmasını dileriz.

 [1]: http://www.google.com/analytics/