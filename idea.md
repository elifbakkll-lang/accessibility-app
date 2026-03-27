# idea.md: yol arkadaşı projesi

## 1. problem
engelli bireyler şehir içinde bir noktadan diğerine giderken yolların ve mekanların erişilebilirlik durumu hakkında güncel bilgiye sahip değiller. mevcut harita uygulamaları "basamak var mı?", "rampa eğimi uygun mu?" gibi detayları sağlamakta yetersiz kalıyor.

## 2. kullanıcılar
* **birincil kullanıcı (engelli birey):** navigasyon ve güvenli rota planlama için kullanan hedef kitle.
* **ikincil kullanıcı (katkıda bulunan):** fotoğraf çekerek ve veri girerek sistemin veri tabanını güncel tutan gönüllüler.

## 3. ai'ın (yz) rolü
* **görüntü sınıflandırma:** kullanıcıların yüklediği fotoğrafları analiz ederek rampa, asansör gibi öğeleri otomatik doğrular.
* **akıllı erişilebilirlik skoru:** formül aracılığıyla her mekana dinamik bir puan atar.
* **rota planlama:** merdivenleri filtreleyen özel rotalar çizer.

## 4. rakip durum ve farkımız
* **rakipler:** wheelmap, accessnow, google maps, wewalk.
* **farkımız:** yz ile anlık fotoğraf doğrulaması, kişiye özel engel profili ve yerel (türkiye) veri derinliği.

## 5. başarı kriteri
bir engelli bireyin uygulamayı açıp, engelsiz rotasını 30 saniye içinde oluşturabilmesi.
