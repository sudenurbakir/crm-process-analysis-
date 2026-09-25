# User Acceptance Testing (UAT)

## 1. Amaç

Bu doküman, CRM sisteminin temel iş ihtiyaçlarını karşılayıp karşılamadığını kullanıcı perspektifinden kontrol etmek amacıyla hazırlanmıştır.

UAT, sistemin teknik olarak çalışmasından çok **iş sürecine uygun olup olmadığını** kontrol eder.

---

## 2. UAT Senaryoları

| ID     | UAT Senaryosu                                | Beklenen Sonuç                                   |
| ------ | -------------------------------------------- | ------------------------------------------------ |
| UAT-01 | Yeni Lead oluşturma                          | Lead başarıyla oluşturulmalı                     |
| UAT-02 | Lead'i Qualified olarak işaretleme           | Lead Qualified durumuna geçmeli                  |
| UAT-03 | Qualified Lead'i Opportunity'ye dönüştürme   | Opportunity oluşturulmalı                        |
| UAT-04 | Opportunity'yi Pipeline'da takip etme        | Opportunity doğru aşamada görüntülenmeli         |
| UAT-05 | Opportunity'yi Won/Lost olarak sonuçlandırma | Sonuç ve gerekli bilgiler kaydedilmeli           |
| UAT-06 | Geçmiş aktiviteleri görüntüleme              | Lead/Opportunity iletişim geçmişi görüntülenmeli |

---

## 3. UAT Kabul Kriterleri

CRM sistemi aşağıdaki koşulları sağladığında iş birimi tarafından kabul edilebilir:

* Lead kayıtları oluşturulabilmeli.
* Lead'ler değerlendirilebilmeli.
* Qualified Lead'ler Opportunity'ye dönüştürülebilmeli.
* Opportunity'ler Pipeline üzerinden takip edilebilmeli.
* Won/Lost sonuçları kaydedilebilmeli.
* Lead ve Opportunity aktiviteleri takip edilebilmeli.

---

## 4. UAT Sonucu

| Durum   | Açıklama                  |
| ------- | ------------------------- |
| Passed  | İş ihtiyacı karşılanıyor  |
| Failed  | İş ihtiyacı karşılanmıyor |
| Blocked | Test gerçekleştirilemiyor |

UAT sonucunda tüm kritik iş akışları başarılı olduğunda sistemin kullanıcı kabul sürecinin tamamlandığı değerlendirilir.
