# TO-BE Process

## 1. Genel Bakış

TO-BE Process, mevcut sürecin iyileştirilmesi sonrasında hedeflenen yeni iş sürecini ifade eder.

Bu projede CRM sisteminin kullanılmasıyla Lead ve Opportunity süreçlerinin merkezi, standart ve izlenebilir hale getirilmesi hedeflenmektedir.

Temel süreç:

**Lead Oluşturma → Lead Atama → Değerlendirme → İletişim → Nitelendirme → Opportunity → Sales Pipeline → Kazanıldı / Kaybedildi**

---

## 2. TO-BE Süreç Akışı

Yeni süreçte Lead'lerin merkezi CRM sistemi üzerinden yönetilmesi planlanmaktadır.

```text id="5z9f3k"
Lead Kaynağı
      ↓
CRM'de Lead Oluşturma
      ↓
Lead Bilgilerinin Kontrolü
      ↓
Lead Atama
      ↓
Lead Değerlendirme
      ↓
Müşteriyle İletişim
      ↓
Aktivite Kaydı
      ↓
Lead Nitelendirme
      ↓
 ┌───────────────┐
 │               │
Nitelikli      Niteliksiz
 │               │
 ↓               ↓
Opportunity     Lead Kapatma
 │
 ↓
Sales Pipeline
 │
 ↓
İhtiyaç Analizi
 │
 ↓
Teklif
 │
 ↓
Müzakere
 │
 ┌───────┴───────┐
 ↓               ↓
Kazanıldı      Kaybedildi
```

---

## 3. Adım 1 — Lead'in CRM'e Gelmesi

Potansiyel müşteriden gelen bilgiler CRM sistemine Lead olarak kaydedilir.

Lead aşağıdaki kanallardan gelebilir:

* Web sitesi
* E-posta
* Telefon
* Sosyal medya
* Referans
* Etkinlik

Lead kaynağı sistem üzerinde ayrıca tutulur.

Böylece Lead'in hangi kanaldan geldiği daha sonra raporlanabilir.

---

## 4. Adım 2 — Lead Bilgilerinin Kontrolü

Lead oluşturulurken sistem zorunlu alanların doldurulup doldurulmadığını kontrol eder.

Örneğin:

* Ad Soyad
* E-posta
* Telefon
* Şirket
* Lead Kaynağı

gibi bilgiler eksikse sistem kullanıcıyı uyarır.

Amaç, eksik ve standart dışı kayıtların oluşmasını azaltmaktır.

---

## 5. Adım 3 — Lead Atama

Lead uygun satış temsilcisine atanır.

Atama sonrasında:

**Lead → Sorumlu Sales Representative**

ilişkisi oluşturulur.

Satış temsilcisi kendi sorumluluğundaki Lead'leri CRM üzerinden görebilir.

Satış yöneticisi ise ekipteki Lead'lerin dağılımını takip edebilir.

---

## 6. Adım 4 — Lead Değerlendirme

Satış temsilcisi CRM üzerinden Lead'i inceler.

Aşağıdaki bilgiler değerlendirilir:

* Müşteri ihtiyacı
* Ürün ilgisi
* İletişim durumu
* Potansiyel satın alma
* Zamanlama
* Mevcut müşteri bilgileri

Eksik bilgiler varsa Lead kaydı güncellenir.

---

## 7. Adım 5 — Müşteriyle İletişim

Satış temsilcisi müşteriyle iletişime geçer.

Yapılan görüşme CRM üzerinde aktivite olarak kaydedilir.

Örneğin:

**Aktivite Türü:** Telefon
**Tarih:** 22.09.2026
**Açıklama:** Müşterinin CRM çözümüyle ilgilendiği ve teklif talep ettiği bilgisi kaydedildi.

Bu sayede müşteriyle yapılan işlemler tek bir kayıt üzerinde takip edilebilir.

---

## 8. Adım 6 — Lead Nitelendirme

İletişim ve değerlendirme sonrasında Lead'in satış fırsatına dönüşmeye uygun olup olmadığı belirlenir.

### Nitelikli Lead

Lead'in gerçek bir ihtiyacı ve satış potansiyeli varsa:

**Lead → Nitelikli**

olarak işaretlenir.

Ardından Opportunity'ye dönüştürülür.

### Niteliksiz Lead

Satış potansiyeli bulunmuyorsa:

**Lead → Niteliksiz**

olarak işaretlenir ve süreç kapatılır.

---

## 9. Adım 7 — Opportunity Oluşturma

Nitelikli Lead Opportunity'ye dönüştürülür.

Örneğin:

**Lead:**

> ABC Teknoloji

↓

**Opportunity:**

> ABC Teknoloji – CRM Lisans Satışı

Opportunity ile birlikte:

* Müşteri
* Sorumlu satış temsilcisi
* Tahmini değer
* Beklenen kapanış tarihi
* Satış aşaması

gibi bilgiler takip edilir.

---

## 10. Adım 8 — Sales Pipeline Takibi

Opportunity oluşturulduktan sonra satış süreci pipeline üzerinden takip edilir.

Aşamalar:

**Yeni Fırsat**

↓

**İhtiyaç Analizi**

↓

**Teklif**

↓

**Müzakere**

↓

**Kazanıldı / Kaybedildi**

Her aşama Opportunity'nin mevcut durumunu gösterir.

---

## 11. Adım 9 — Kazanılan Opportunity

Müşteri satın alma kararını verdiğinde Opportunity:

**Kazanıldı**

olarak işaretlenir.

Bu bilgi satış raporlarına dahil edilir.

Örneğin:

* Kazanılan fırsat sayısı
* Kazanılan fırsatların toplam değeri
* Satış temsilcisi bazında kazanılan fırsatlar

analiz edilebilir.

---

## 12. Adım 10 — Kaybedilen Opportunity

Satış gerçekleşmezse Opportunity:

**Kaybedildi**

olarak işaretlenir.

Kullanıcıdan mümkün olduğunda kayıp nedeni girmesi istenir.

Örneğin:

* Fiyat
* Rakip
* Bütçe
* Zamanlama
* İhtiyacın ortadan kalkması

Bu bilgiler daha sonra kayıp analizi için kullanılabilir.

---

## 13. AS-IS → TO-BE Dönüşümü

| AS-IS                            | TO-BE                            |
| -------------------------------- | -------------------------------- |
| Excel ve e-posta kullanımı       | Merkezi CRM                      |
| Manuel Lead kaydı                | Standart Lead formu              |
| Manuel takip                     | CRM aktivite takibi              |
| Kişisel notlar                   | Merkezi müşteri geçmişi          |
| Manuel Lead atama                | CRM üzerinden sorumluluk         |
| Dağınık Opportunity takibi       | Sales Pipeline                   |
| Standart olmayan durumlar        | Tanımlı Lead Status              |
| Standart olmayan satış aşamaları | Tanımlı Opportunity Stage        |
| Kayıp nedenleri dağınık          | Standart kayıp nedenleri         |
| Manuel raporlama                 | CRM verileri üzerinden raporlama |

---

## 14. TO-BE Sürecinin Sağladığı Faydalar

### Merkezi Veri

Lead ve Opportunity bilgileri tek bir sistemde tutulur.

### Standart Süreç

Tüm satış temsilcileri aynı temel süreç üzerinden ilerler.

### İzlenebilirlik

Lead'in ve Opportunity'nin geçmiş işlemleri takip edilebilir.

### Sorumluluk Takibi

Her Lead ve Opportunity için sorumlu kişi belirlenebilir.

### Pipeline Görünürlüğü

Satış yöneticileri fırsatların hangi aşamada olduğunu görebilir.

### Raporlama

CRM'de bulunan veriler kullanılarak temel satış raporları oluşturulabilir.

---

## 15. BA Açısından TO-BE Analizi

Business Analyst, TO-BE süreci tasarlarken aşağıdaki sorulara cevap verir:

### Süreç

* Yeni süreç nasıl çalışacak?
* Hangi adımlar sistem tarafından desteklenecek?
* Hangi adımlar kullanıcı tarafından gerçekleştirilecek?

### İş Kuralları

* Lead ne zaman Opportunity'ye dönüşebilir?
* Hangi Lead durumlarında dönüşüm engellenmeli?
* Opportunity hangi koşulda kazanıldı olarak işaretlenebilir?
* Kaybedilen fırsatta hangi bilgiler zorunlu olmalı?

### Sistem

* Hangi alanlar zorunlu?
* Kim hangi kaydı görebilir?
* Kim hangi alanı değiştirebilir?
* Hangi aktiviteler kayıt altına alınmalı?

### Veri

* Lead'den Opportunity'ye hangi bilgiler aktarılacak?
* Müşteri ve kişi bilgileri nasıl ilişkilendirilecek?
* Hangi bilgiler raporlamada kullanılacak?

---

## 16. TO-BE Başarı Kriterleri

Yeni sürecin başarılı kabul edilebilmesi için:

* Lead'ler CRM üzerinde standart şekilde oluşturulabilmeli.
* Her Lead için sorumlu kişi belirlenebilmeli.
* Lead durumları sistem üzerinden takip edilebilmeli.
* Müşteri aktiviteleri kaydedilebilmeli.
* Nitelikli Lead'ler Opportunity'ye dönüştürülebilmeli.
* Opportunity'ler pipeline üzerinden takip edilebilmeli.
* Kazanılan ve kaybedilen fırsatlar kayıt altına alınabilmeli.
* Kayıp nedenleri analiz edilebilmeli.
* Temel satış raporları CRM verileri üzerinden oluşturulabilmeli.

---

## 17. Süreç Özeti

Yeni CRM sürecinin temel mantığı:

**Lead'i merkezi olarak kaydet → Sorumlu ata → Değerlendir → İletişim geçmişini kaydet → Nitelendir → Opportunity'ye dönüştür → Pipeline'da takip et → Satış sonucunu kaydet**

Bu yapı, mevcut dağınık sürecin standart ve izlenebilir bir CRM sürecine dönüştürülmesini sağlar.
