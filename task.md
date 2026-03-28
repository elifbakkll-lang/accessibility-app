# Yol Arkadaşı — Geliştirme Görev Listesi (PRD’ye göre)

Bu liste `prd.md` içeriğine göre öncelik sırasıyla düzenlenmiştir. Her faz tamamlandıkça işaretlenebilir (`[ ]` → `[x]`).

---

## Faz 0 — Ürün ve teknik temel

- [ ] **0.1** Teknik kararları netleştir: PWA önceliği mi, Flutter önceliği mi; tek kod tabanı mı, iki istemci mi (PRD: PWA + Flutter hibrit).
- [ ] **0.2** Depo yapısı: monorepo veya ayrı paketler (`web/`, `mobile/`, `api/`), ortak tipler ve API sözleşmesi.
- [ ] **0.3** Geliştirme ortamı: Node/Pnpm veya benzeri; Flutter SDK sürümü; Docker ile PostgreSQL + PostGIS yerel kurulum.
- [ ] **0.4** Tasarım sistemi / erişilebilir UI ilkeleri: kontrast, ekran okuyucu, odak sırası (ürünün kendisi erişilebilir olmalı).

---

## Faz 1 — Veri modeli ve backend iskeleti

- [ ] **1.1** PostgreSQL + PostGIS kurulumu; coğrafi indeks ve temel şema tasarımı.
- [ ] **1.2** Çekirdek varlıklar: Kullanıcı, Rol (`engelli` / `gonullu`), Engel profili tipleri (akülü sandalye, görme engelli vb.).
- [ ] **1.3** POI (mekan) modeli: tür (kafe, kütüphane, tuvalet, asansör…), konum, erişilebilirlik alanları, son güncelleme zamanı.
- [ ] **1.4** Fotoğraf / kanıt kaydı: POI veya “geçiş noktası”na bağlı; yükleme zamanı; “son 24 saat” sorguları için alanlar.
- [ ] **1.5** Kimlik doğrulama ve yetkilendirme: rol bazlı erişim, güvenli API.

---

## Faz 2 — Harita ve filtreleme (3.1 — kısmi MVP)

- [ ] **2.1** Harita görünümü: OSM tabanlı harita entegrasyonu (web ve/veya mobil).
- [ ] **2.2** Sadece erişilebilir POI’leri gösterme: filtreler (durak, tuvalet, asansör, kafe vb.).
- [ ] **2.3** POI detay ekranı: meta veri + varsa son fotoğraf önizlemesi (“güven kanıtı” için temel).
- [ ] **2.4** Engel profiline göre filtre/görünürlük (basamak, dar kaldırım, dik yokuş vb. — veri modeli ve UI bağlantısı).

---

## Faz 3 — Rota motoru (3.1 — navigasyon)

- [ ] **3.1** GraphHopper (veya eşdeğer) kurulumu; OSM grafı ve özel kısıtlar için strateji.
- [ ] **3.2** Erişilebilirlik kısıtları: merdiven/basamak hariç tutma, eğim eşikleri, yüzey tipi (veri kaynağı ve modelleme).
- [ ] **3.3** “Kısa yol” isteği: başlangıç/bitiş, kullanıcı profili → GraphHopper parametreleri.
- [ ] **3.4** Rota çizimi ve yön adımları; offline gereksinimi PRD’de yoksa sonraki iterasyona bırakılabilir.

---

## Faz 4 — Gönüllü akışı (2.2, ilişkili 3.1)

- [ ] **4.1** Fotoğraf yükleme: konum EXIF / manuel POI seçimi, yetki kontrolleri.
- [ ] **4.2** Yüklenen medyanın sunucuya güvenli aktarımı ve depolama (ör. nesne depolama).
- [ ] **4.3** POI veya “yol üstü engel” kaydı ile ilişkilendirme; gönüllü puan alanının veri modeli (ham puan olayları).
- [ ] **4.4** Son 24 saat içinde çekilmiş görsel vurgusu (liste/harita detayında).

---

## Faz 5 — AI Guardian (3.2 — otomatik doğrulama)

- [ ] **5.1** Google Vision API (veya seçilen model) entegrasyonu; gizlilik ve maliyet kontrolleri.
- [ ] **5.2** Çıktı şeması: rampa var/yok, eğim uyarısı, engel teşkil eden unsur vb. (PRD maddeleriyle hizalama).
- [ ] **5.3** İnsan onayı / düşük güven eşiği iş akışı (yanlış pozitif/negatif için).
- [ ] **5.4** POI veya rapor kaydına AI sonuçlarının yazılması ve istemcide gösterim.

---

## Faz 6 — Belediye entegrasyonu ve raporlama (3.2)

- [ ] **6.1** “Kanıtlı Denetim Raporu” veri modeli: konum, görsel kanıt, açıklama, zaman damgası, AI onayı.
- [ ] **6.2** Engelli kullanıcıdan rapor oluşturma akışı (bozuk asansör, işgal rampa vb.).
- [ ] **6.3** Belediyeye iletim: başlangıçta e-posta/PDF export veya partner API; gerçek entegrasyon partnerine göre genişletilir.
- [ ] **6.4** (İleri) Kamu/ulaşım API’leri: asansör durumu, engelli dostu araç takibi — entegrasyon özeti ve mock.

---

## Faz 7 — İyilik Kumbarası ve şeffaflık (3.3)

- [ ] **7.1** Puan ticaret modeli: İyilik Puanı kazanma kuralları (fotoğraf, doğrulama vb.).
- [ ] **7.2** Puan kullanımı / bağış havuzu: kurumsal ortak (akredite dernek) süreçleri için yer tutucu ve yasal metin alanı.
- [ ] **7.3** Şeffaf takip: medikal cihaz seri no, teslimat belgesi referansı — yetkili roller için görünürlük.
- [ ] **7.4** Engelli kullanıcı tarafında “Erişilebilirlik Elçisi” / gönüllü tarafında rozet veya unvan gösterimi.

---

## Faz 8 — PWA ve Flutter (4. teknik)

- [ ] **8.1** PWA: manifest, service worker, temel kurulum ekranı.
- [ ] **8.2** Flutter: paylaşılan API istemcisi, harita ve auth ekranları; mümkünse iş mantığının backend’de toplanması.
- [ ] **8.3** Bildirimler (rapor durumu, rota uyarıları) — platform izinleri.

---

## Faz 9 — Başarı ölçümleri (5.)

- [ ] **9.1** Olay kaydı: rota kesintisi (kullanıcı “engel nedeniyle rota değiştirdi” bildirimi).
- [ ] **9.2** Panolar: aylık medikal bağış sayısı, belediye rapor geri dönüş oranı için veri toplama ve basit raporlama.

---

## Faz 10 — Güvenlik, uyumluluk ve yayın

- [ ] **10.1** KVKK / gizlilik: konum ve fotoğraf için açık rıza ve saklama süreleri.
- [ ] **10.2** Oran sınırlama, kötüye kullanım önleme (spam fotoğraf/rapor).
- [ ] **10.3** Üretim dağıtımı: API barındırma, yedekleme, izleme (log/metrics).

---

## MVP önerisi (ilk canlı sürüm kapsamı)

PRD’nin tamamı büyük; hızlı değer için önerilen sıra:

1. Faz 0–1–2 (temel + harita + erişilebilir POI).
2. Faz 3’ün sadeleştirilmiş hali (basit engelli-dostu rota, tek profil).
3. Faz 4’ün fotoğraf yükleme + listeleme kısmı.
4. Faz 5’in minimal sürümü (tek etiket doğrulama veya manuel + AI asistan).

`idea.md` başarı kriteri: *“engelli bireyin uygulamayı açıp engelsiz rotayı ~30 saniyede oluşturması”* — Faz 2 + basitleştirilmiş Faz 3 ile ölçülebilir hale getirilmelidir.

