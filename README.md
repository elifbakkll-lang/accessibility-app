
# 💡 Yol Arkadaşı: Engelsiz Şehir & İyilik Ekosistemi

**Yol Arkadaşı**, şehir mimarisindeki fiziksel engelleri dijital bir dayanışma ağıyla görünür kılan; engelli bireylerin özgürlüğünü toplumun kolektif **"iyilik gücüyle"** birleştiren bir sosyal inovasyon platformudur.

---

## 🚀 Canlı Demo & Proje Linkleri

* **Ana Uygulama (Level 1 - MVP):** [yolarkadasin.lovable.app](https://yolarkadasin.lovable.app)
* **Kaynak Kodlar (v2):** [github.com/elifbakkll-lang/v2.yolarkadasin](https://github.com/elifbakkll-lang/v2.yolarkadasin)

---

## 🧠 Problem ve Çözüm

### Problem: Şehirdeki "Görünmez" Bariyerler
Mevcut haritalar; dik rampa eğimlerini, bozuk asansörleri veya dar kaldırımları filtrelemez. Bu durum, engelli bireyler için ulaşımı bir navigasyon sorunundan ziyade bir **belirsizlik** sorununa dönüştürür.

### Çözüm: Bütünleşik Erişilebilirlik Ağı
* **Kesintisiz Koridor:** Engel grubuna göre özelleştirilmiş; basamak, dik eğim ve dar kaldırım içermeyen rotalar.
* **Görsel Kanıt:** Rota üzerindeki kritik noktaların gönüllülerce çekilmiş güncel fotoğrafları ile anlık doğrulama.
* **İyilik Kumbarası:** Gönüllülerin veri girişlerini (fotoğraf, rapor) somut medikal yardımlara (tekerlekli sandalye vb.) dönüştüren etik döngü.

---

## 🤖 AI Guardian: Yapay Zeka Ne Yapıyor?
Projenin merkezindeki AI katmanı şu kritik görevleri üstlenir:

* **Görsel Doğrulama:** Yüklenen fotoğrafların gerçekten rampa veya asansör içerip içermediğini nesne tanıma (**Object Detection**) ile analiz eder.
* **Akıllı Puanlama:** Güzergahın "Erişilebilirlik Skorunu" hesaplar ve anlık verilere (bozuk asansör bildirimi vb.) göre rotayı dinamik günceller.
* **Sahtecilik Engelleme:** Sisteme yüklenen hatalı veya kopya verileri ayıklayarak iyilik puanı sisteminin güvenliğini sağlar.

---

## 🛠️ Teknik Altyapı (Tech Stack)

### Frontend & Prototipleme
* **Lovable:** Hızlı MVP üretimi ve React tabanlı arayüz bileşenleri için AI-driven platform.
* **Tailwind CSS:** Erişilebilirlik (**WCAG 2.1**) standartlarına uygun, yüksek kontrastlı UI.

### Backend & Navigasyon
* **Supabase / PostgreSQL:** Gerçek zamanlı veri yönetimi ve coğrafi (**PostGIS**) sorgular.
* **Mapbox SDK / OSM:** Özel kısıtlar (eğim, zemin tipi) eklenmiş navigasyon motoru.
* **Google Vision API:** Görüntü işleme ve nesne tanıma.

---

## 👨‍💻 Nasıl Çalıştırılır?

Bu projeyi yerel ortamınızda ayağa kaldırmak için aşağıdaki adımları takip edin:

1.  **Depoyu Klonlayın:**
    ```bash
    git clone https://github.com/elifbakkll-lang/v2.yolarkadasin.git
    cd v2.yolarkadasin
    ```
2.  **Bağımlılıkları Yükleyin:**
    ```bash
    npm install
    ```
3.  **Uygulamayı Başlatın:**
    ```bash
    npm run dev
    ```

---

## 🎯 Başarı Kriterimiz
Bir engelli bireyin, evinden çıkıp gitmek istediği noktaya hiçbir fiziksel engelle karşılaşmadan ve toplumsal dayanışmayı hissederek **30 saniye içinde** güvenli rotasını oluşturabilmesi.

---
*Bu proje, şehirleri herkes için daha yaşanabilir kılmak adına bir teknoloji ve vicdan köprüsü kurmayı hedefler.*
