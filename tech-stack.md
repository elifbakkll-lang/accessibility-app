# 🛠️ yol arkadaşı: teknik altyapı (tech stack)

bu döküman, projenin geliştirme görev listesinde (roadmap) yer alan fazların hayata geçirilmesi için seçilen teknolojileri, kütüphaneleri ve mimari tercihleri detaylandırır.

---

## ⚡ hızlı prototipleme & frontend üretimi (ai-driven)
projenin görsel arayüzlerinin ve ilk çalışan prototiplerinin (mvp) hızla hayata geçirilmesi için seçilen ana araç:

* **geliştirme platformu:** lovable (ai-powered full-stack app builder).
* **kullanım amacı:** hızlı pwa (progressive web app) üretimi, react tabanlı arayüz bileşenlerinin oluşturulması ve frontend-backend entegrasyonunun ilk aşaması.
* **avantaj:** tasarımdan koda geçiş süresini %80 oranında azaltarak, "kesintisiz koridor" vizyonunun görselleştirilmesini sağlar.

---

## 📱 frontend (mobil & web) - [faz 0 & faz 8]
uygulamanın hem ios/android hem de web üzerinde tek bir kod tabanıyla çalışması ve en yüksek erişilebilirlik standartlarını karşılaması için:

* **framework:** flutter (hibrit mobil uygulama; prd'de belirtilen pwa + flutter hibrit yapısı için).
* **state management:** bloc veya riverpod (karmaşık rota ve iyilik puanı verilerini yönetmek için).
* **web desteği:** pwa (progressive web app) teknolojisi ile tarayıcı üzerinden hızlı erişim ve manifest desteği.
* **erişilebilirlik:** wcag 2.1 uyumlu ui bileşenleri, talkback/voiceover desteği.

---

## ⚙️ backend (api & sunucu) - [faz 1]
hızlı veri işleme, coğrafi doğrulama ve güvenli raporlama süreçleri için:

* **runtime:** node.js (asenkron işlem kapasitesi ile yüksek performans).
* **framework:** nestjs (belediye ve ai entegrasyonları için ölçeklenebilir mimari).
* **veritabanı:** postgresql (ilişkisel veri yönetimi).
* **coğrafi eklenti:** postgis (faz 1.1; koordinat bazlı sorgular ve "erişilebilir POI" filtrelemesi için zorunlu).
* **orm:** prisma (api sözleşmesi ve veri güvenliği için).

---

## 🗺️ harita & navigasyon - [faz 2 & faz 3]
"kesintisiz koridor" vizyonunu ve engelsiz rota algoritmalarını çalıştırmak için:

* **harita sağlayıcı:** mapbox sdk veya openstreetmap (osm).
* **routing engine:** graphhopper (faz 3.1; basamak, yokuş ve dar kaldırım kısıtlarını içeren özel rota motoru).

---

## 🤖 yapay zeka & doğrulama (ai guardian) - [faz 5]
gönüllülerden gelen görsellerin sahteciliğe karşı korunması ve içerik analizi için:

* **bulut api:** google vision api (rampa, asansör ve engel tespiti için ilk aşama entegrasyonu).
* **metadata analizi:** exif veri kontrolü (fotoğrafın çekildiği yer ve zaman doğrulaması için).

---

## ☁️ altyapı & güvenlik - [faz 10]
* **kimlik doğrulama:** firebase auth (rol bazlı erişim yönetimi).
* **konteynırlaştırma:** docker (faz 0.3; yerel geliştirme ortamı ve postgis kurulumu için).
* **ci/cd:** github actions (otomatik test ve dağıtım süreçleri).
