Harika, eklediğin yeni bilgilerle projenin gelişim sürecini (v1, Claude prototipi ve Buildathon sunumu) kapsayan, çok daha güçlü ve detaylı bir `README.md` hazırladım. Bu versiyon, projenin sadece bir fikir değil, farklı araçlarla (Lovable, Claude, Vercel) test edilmiş ve olgunlaşmış bir çözüm olduğunu gösteriyor.

İşte kopyalayıp kullanabileceğin güncel format:

---

# 💡 Yol Arkadaşı: Engelsiz Şehir & İyilik Ekosistemi

**Yol Arkadaşı**, şehir mimarisindeki fiziksel engelleri dijital bir dayanışma ağıyla görünür kılan; engelli bireylerin özgürlüğünü toplumun kolektif **"iyilik gücüyle"** birleştiren bir sosyal inovasyon platformudur. "Her adım herkes için" diyerek şehri sürprizlerden arındırılmış kesintisiz bir koridora dönüştürmeyi amaçlar.

---

## 🚀 Canlı Demo & Proje Linkleri

* **Ana Uygulama (Level 1 - MVP):** [yolarkadasin.lovable.app](https://yolarkadasin.lovable.app)
* **Geliştirme Versiyonu (Vercel):** [v0-accessibility-map-app.vercel.app](https://v0-accessibility-map-app-iota.vercel.app)
* **Geliştirme Versiyonu (Claude):** [file:///C:/Users/ASUS/Downloads/accessibility_map_app_v2%20(2).html]
* **Kaynak Kodlar (v2):** [github.com/elifbakkll-lang/v2.yolarkadasin](https://github.com/elifbakkll-lang/v2.yolarkadasin)
* **Sunum & Demo Videosu (BGK'26 AI Buildathon):** [YouTube İzle](https://youtu.be/1gxQ0hPXbEc?si=w9w8jdGBoCayBhej)

---

## 🧠 Problem ve Çözüm

### Problem: Şehirdeki "Görünmez" Bariyerler
Mevcut haritalar; dik rampa eğimlerini, bozuk asansörleri veya dar kaldırımları filtrelemez. Bu durum, engelli bireyler için ulaşımı bir navigasyon sorunundan ziyade bir **belirsizlik** sorununa dönüştürür.

### Çözüm: Bütünleşik Erişilebilirlik Ağı
* **Kesintisiz Koridor:** Kullanıcının engel grubuna göre özelleştirilmiş; basamak, dik eğim ve dar kaldırım içermeyen rotalar.
* **Görsel Kanıt:** Rota üzerindeki kritik noktaların gönüllülerce çekilmiş güncel fotoğrafları ile anlık doğrulama.
* **İyilik Kumbarası:** Gönüllülerin veri girişlerini (fotoğraf, rapor) puanlara dönüştürerek tekerlekli sandalye veya protez gibi somut medikal yardımlara vesile olan etik döngü.

---

## 🤖 AI Guardian & Teknoloji Deneyimi
Bu proje, BGK'26 AI Buildathon sürecinde farklı yapay zeka araçlarının birleşimiyle geliştirilmiştir:

* **Görsel Doğrulama (AI Guardian):** Yüklenen fotoğrafların gerçekten rampa veya asansör içerip içermediğini nesne tanıma ile analiz eder.
* **Akıllı Raporlama:** Yapay zeka onaylı engel raporları, yerel yönetim sistemlerinde önceliklendirilerek fiziksel onarım sürecini hızlandırır.
* **Çoklu Model Kullanımı:** PRD süreçlerinde Gemini, uygulama gereksinimleri ve prototipleme aşamasında Claude, V0 ve Cursor kullanılmış; nihai MVP Lovable üzerinde finalize edilmiştir.

---

## 🛠️ Teknik Altyapı (Tech Stack)

* **Frontend:** Lovable (React tabanlı), Vercel Deployment.
* **Tasarım:** WCAG 2.1 uyumlu erişilebilir arayüz ve Tailwind CSS.
* **Backend & Veri:** Supabase / PostgreSQL (PostGIS coğrafi sorgular).
* **Navigasyon:** Mapbox SDK / OSM (Eğim ve zemin tipi kısıtlamalı özel rota motoru).
* **AI:** Google Vision API ve özel eğitilmiş nesne tanıma modelleri.

---

## 👨‍💻 Nasıl Çalıştırılır?

Bu projeyi yerel ortamınızda ayağa kaldırmak için:

1.  **Depoyu Klonlayın:**
    ```bash
    git clone https://github.com/elifbakkll-lang/v2.yolarkadasin.git
    cd v2.yolarkadasin
    ```
2.  **Bağımlılıkları Yükleyin:** `npm install`
3.  **Uygulamayı Başlatın:** `npm run dev`

---

## 🎯 Başarı Kriterimiz
Bir engelli bireyin, evinden çıkıp gitmek istediği noktaya hiçbir fiziksel engelle karşılaşmadan ve toplumsal dayanışmayı hissederek **30 saniye içinde** güvenli rotasını oluşturabilmesi.

---
*Engeller paylaştıkça azalır, yollar paylaştıkça kısalır.*



http://googleusercontent.com/youtube_content/7
