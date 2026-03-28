# 🗺️ Yol Arkadaşı: Kullanıcı Akış Şeması (User Flow)

Bu döküman, uygulamadaki iki temel kullanıcı grubunun (Engelli Kullanıcı ve Gönüllü Kullanıcı) deneyim adımlarını ve sistemin bu adımlara verdiği yanıtları tanımlar.

---

## 👨‍🦽 1. Senaryo: Engelli Kullanıcı (Kesintisiz Navigasyon)

Engelli bireyin evinden çıkıp, hedefine hiçbir sürprizle karşılaşmadan ulaşma sürecidir.

1. **Giriş & Profil:**
   * kullanıcı uygulamayı açar.
   * engel tipini seçer (tekerlekli sandalye, görme engelli, yürüme zorluğu vb.).
2. **Hedef Arama:**
   * arama çubuğuna gitmek istediği yeri (kafe, kütüphane, kamu binası) yazar.
3. **Erişilebilirlik Filtreleme:**
   * sistem, sadece kullanıcının engel grubuna uygun olan "erişilebilir durakları" haritada listeler.
4. **Rota Oluşturma:**
   * yapay zeka; basamak, dik eğim ve dar kaldırımları devre dışı bırakarak **"kesintisiz koridor"** rotasını çizer.
5. **Görsel Doğrulama:**
   * kullanıcı rota üzerindeki kritik noktaların (rampa, asansör) gönüllülerce çekilmiş **güncel fotoğraflarını** önizler.
6. **Navigasyon & Denetim:**
   * kullanıcı yola çıkar. yol üzerinde bir engel (hatalı park, bozuk asansör) görürse **"belediyeye bildir"** butonuyla kanıtlı rapor oluşturur.
7. **Varış & Puanlama:**
   * hedefe ulaştığında mekanın erişilebilirliğini puanlar ve **"erişilebilirlik elçisi"** puanı kazanır.

---

## 🤝 2. Senaryo: Gönüllü Kullanıcı (İyilik Elçisi)

Toplumsal dayanışmaya katkı sağlamak isteyen kullanıcının veri toplama ve bağış sürecidir.

1. **Keşif Modu:**
   * gönüllü uygulamayı açar ve çevresindeki "onay bekleyen" veya "fotoğrafı eksik" noktaları haritada görür.
2. **Aktif Veri Toplama:**
   * kullanıcı hem haritada belirlenen eksik noktalara gider hem de kendi güzergahı üzerinde fark ettiği tüm erişilebilirlik detaylarının (rampa, asansör, girişler) fotoğrafını çeker.
3. **AI Denetimi:**
   * yapay zeka fotoğrafı analiz eder. nesne tanıma ile verinin doğruluğunu ve rampa/asansör uygunluğunu onaylar.
4. **İyilik Puanı Kazanımı:**
   * onaylanan her veri girişi için kullanıcı profilinde **"iyilik puanı"** birikir.
5. **Kumbaraya Bağış:**
   * kullanıcı "iyilik kumbarası" ekranına girer. biriken puanlarını aktif olan bağış hedefine (örn: "tekerlekli sandalye bağışı") aktarır.
6. **Şeffaf Geri Bildirim:**
   * bağış hedefi tamamlandığında kullanıcıya **"sayende bir hayat değişti!"** bildirimi ve dijital sertifikası iletilir.

---

## ⚙️ 3. Arka Plan Sistem Akışı (System Logic)

* **Veri Senkronizasyonu:** gönüllüden gelen veri onaylandığı an, engelli kullanıcının haritası dinamik olarak güncellenir.
* **Resmi Raporlama:** olumsuz bildirimler (bozuk rampa vb.), sistem tarafından otomatik olarak belediye fen işleri formatına dönüştürülüp iletilir.
* **Bağış Tetikleyici:** kumbara dolduğunda anlaşmalı dernekler (tofd, girvak vb.) üzerinden cihaz tedarik süreci başlatılır.
