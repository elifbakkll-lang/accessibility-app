# 🛡️ Yol Arkadaşı: (Bütünleşik Erişilebilirlik Ağı & Sosyal İyilik Ekosistemi)

## 1. Vizyon ve Sosyal Misyon
**Yol Arkadaşı**, şehir mimarisindeki engelleri dijital bir dayanışma ağıyla görünür kılan; engelli bireylerin özgürlüğünü kısıtlayan fiziksel engelleri toplumun kolektif **"iyilik gücüyle"** ortadan kaldıran bir sosyal dönüşüm platformudur. 

Temel misyonumuz; engelli bireylere evden çıktıkları andan itibaren kesintisiz ve sürprizsiz bir **"erişilebilirlik koridoru"** sunarken, gönüllülerin dijital katkılarını (fotoğraf, veri, doğrulama) somut medikal yardımlara (tekerlekli sandalye, protez vb.) dönüştüren etik bir iyilik döngüsü yaratmaktır.

---

## 2. Kullanıcı Segmentleri ve Rol Tanımları

### 2.1. Engelli Kullanıcılar (Erişilebilirlik Elçileri)
* **Kesintisiz Deneyim:** Engel grubuna göre (akülü sandalye, görme engelli vb.) özelleştirilmiş; basamak, dar kaldırım ve dik yokuş içermeyen rotalar kullanır.
* **Denetçi Rolü:** Karşılaştığı hatalı yapıları (bozuk asansör, işgal edilmiş rampa vb.) YZ onayıyla doğrudan belediyeye raporlar.
* **Motivasyon:** Güvenli ulaşım hakkı, **"Erişilebilirlik Elçisi"** unvanı ve kendi medikal ekipmanları (akü, bakım, aksesuar) için puan tabanlı destek.

### 2.2. Gönüllü Kullanıcılar (İyilik Elçileri)
* **Veri Kaynağı:** Rota üzerindeki mekanların (kafe, kütüphane vb.) ve yoldaki engellerin güncel fotoğraflarını çekerek sistemi besler.
* **Motivasyon:** Kazandığı **"İyilik Puanları"** ile ihtiyaç sahipleri adına tekerlekli sandalye bağışlanmasına, fidan dikilmesine veya tohum topları saçılmasına vesile olur.

---

## 3. Temel Fonksiyonel Katmanlar

### 3.1. Bütünleşik Erişilebilirlik Haritası (POI & Rota)
* **Erişilebilir Duraklar:** Harita üzerinde sadece engelli erişimine uygun; kafeler, kütüphaneler, tuvaletler ve asansörler filtrelenerek gösterilir.
* **Görsel Doğrulama:** Her mekanın ve kritik geçiş noktasının son 24 saat içinde çekilmiş fotoğrafı, kullanıcıya **"güven kanıtı"** olarak sunulur.
* **Kesintisiz Navigasyon:** Mesafe kadar "zemin kalitesini" (eğim analizi, yüzey tipi) de hesaplayan, engelsiz kısa yol algoritmaları.

### 3.2. Yapay Zeka (AI Guardian) ve Belediye Entegrasyonu
* **Otomatik Doğrulama:** Yüklenen fotoğrafların içeriğini (Rampa var mı? Eğimi uygun mu? Engel teşkil ediyor mu?) ve gerçekliğini analiz eder.
* **Dijital Raporlama:** Onaylanan olumsuz durumlar, belediyelerin ilgili birimlerine konumu ve görsel kanıtıyla birlikte **"Kanıtlı Denetim Raporu"** olarak iletilir.
* **Kamu Entegrasyonu:** Belediye ulaşım ağları ile entegre; asansörlerin çalışma durumu ve engelli dostu araçların canlı takibi yapılır.

### 3.3. Etik Bağış ve İyilik Kumbarası
* **Şeffaf Takip:** Toplanan puanlarla alınan medikal cihazların seri numarası ve teslimat belgesi tüm katkı sağlayan gönüllülere iletilir.
* **Kurumsal Ortaklık:** Bağış süreçleri sadece akredite dernekler (Örn: TOFD, GİRVAK) üzerinden, etik kurallar çerçevesinde yürütülür.

---

## 4. Teknik Altyapı
* **Platform:** PWA (Progressive Web App) ve Flutter (Hibrit Mobil).
* **Navigasyon Motoru:** OpenStreetMap (OSM) + GraphHopper (Özel kısıtlar eklenmiş).
* **Veritabanı:** PostgreSQL + PostGIS (Coğrafi sorgular için).
* **AI Katmanı:** Google Vision API veya özel eğitilmiş nesne tanıma modelleri.

---

## 5. Başarı Kriterleri
1.  **Sıfır Kesinti Oranı:** Kullanıcının rotasını fiziksel bir engel nedeniyle değiştirmek zorunda kalmadığı yolculuk yüzdesi.
2.  **Sosyal Etki:** Topluluk tarafından tamamlanan aylık medikal cihaz bağış sayısı.
3.  **Çözüm Hızı:** Belediye birimlerine iletilen raporların geri dönüş ve onarılma oranı.
