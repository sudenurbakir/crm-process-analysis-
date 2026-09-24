# Business Rules

## 1. Genel Bakış

Business Rules, CRM sistemindeki iş süreçlerinin hangi kurallara göre çalışacağını tanımlar.

Bu kurallar, kullanıcıların ve sistemin belirli durumlarda nasıl davranması gerektiğini açıklamaktadır.

---

## 2. Lead Kuralları

### BR-01 — Zorunlu Lead Bilgileri

Lead oluşturulurken aşağıdaki bilgiler zorunlu olmalıdır:

* Ad Soyad
* E-posta veya Telefon
* Şirket
* Lead Kaynağı
* Sorumlu Satış Temsilcisi

Zorunlu bilgiler tamamlanmadan Lead oluşturulmamalıdır.

---

### BR-02 — Lead Sorumlusu

Her Lead'in bir sorumlu satış temsilcisi olmalıdır.

Sorumlusu bulunmayan Lead, takip edilmesi gereken aktif bir kayıt olarak bırakılmamalıdır.

---

### BR-03 — Lead Durumu

Her Lead'in yalnızca bir aktif durumu olmalıdır.

Desteklenen temel durumlar:

* Yeni
* İletişime Geçilecek
* İletişim Kuruldu
* Nitelikli
* Niteliksiz
* Dönüştürüldü
* Kayıp

---

### BR-04 — Lead Durumu Güncelleme

Lead'in durumu gerçekleştirilen işleme göre güncellenmelidir.

Örneğin müşteriyle iletişim kurulduğunda Lead:

**İletişime Geçilecek → İletişim Kuruldu**

şeklinde güncellenebilir.

---

### BR-05 — Niteliksiz Lead Dönüşümü

**Niteliksiz** olarak işaretlenen bir Lead Opportunity'ye dönüştürülememelidir.

---

### BR-06 — Nitelikli Lead Dönüşümü

Opportunity'ye dönüştürülecek Lead'in **Nitelikli** durumda olması gerekmelidir.

---

### BR-07 — Lead Dönüşümünün Tekrarlanmaması

Daha önce Opportunity'ye dönüştürülmüş bir Lead tekrar Opportunity'ye dönüştürülememelidir.

---

## 3. Aktivite Kuralları

### BR-08 — Aktivite İlişkisi

Her aktivite en az bir Lead veya Opportunity ile ilişkilendirilmelidir.

Bağımsız ve hangi müşteri sürecine ait olduğu bilinmeyen aktivite oluşturulmamalıdır.

---

### BR-09 — Aktivite Türü

Aktivitenin bir türü bulunmalıdır.

Desteklenen temel aktivite türleri:

* Telefon
* E-posta
* Toplantı
* Not

---

### BR-10 — Aktivite Tarihi

Her aktivite için tarih bilgisi tutulmalıdır.

Bu bilgi müşteriyle yapılan işlemlerin geçmişinin takip edilmesini sağlar.

---

## 4. Opportunity Kuralları

### BR-11 — Opportunity Sorumlusu

Her Opportunity için bir sorumlu satış temsilcisi bulunmalıdır.

---

### BR-12 — Opportunity Aşaması

Her Opportunity'nin yalnızca bir aktif satış aşaması olmalıdır.

Aşamalar:

1. Yeni Fırsat
2. İhtiyaç Analizi
3. Teklif
4. Müzakere
5. Kazanıldı
6. Kaybedildi

---

### BR-13 — Opportunity Aşama Geçişi

Opportunity, satış sürecine uygun şekilde aşamalar arasında ilerlemelidir.

Temel akış:

**Yeni Fırsat → İhtiyaç Analizi → Teklif → Müzakere**

Sonrasında:

**Kazanıldı** veya **Kaybedildi**

durumlarından biri seçilir.

---

### BR-14 — Kazanılan Opportunity

Opportunity **Kazanıldı** olarak işaretlendiğinde satış süreci tamamlanmış kabul edilir.

Kazanılan Opportunity tekrar aktif bir satış aşamasına alınmamalıdır.

---

### BR-15 — Kaybedilen Opportunity

Opportunity **Kaybedildi** olarak işaretlendiğinde kayıp nedeni belirtilmelidir.

Örnek:

* Fiyat
* Rakip
* Bütçe
* Zamanlama
* İhtiyacın ortadan kalkması

---

### BR-16 — Kapanan Opportunity Güncellemesi

**Kazanıldı** veya **Kaybedildi** durumundaki Opportunity aktif satış fırsatı olarak değerlendirilmemelidir.

---

## 5. Pipeline Kuralları

### BR-17 — Pipeline Görünürlüğü

Aktif Opportunity'ler pipeline içerisinde mevcut aşamalarında görüntülenmelidir.

---

### BR-18 — Pipeline Değeri

Pipeline toplam değeri hesaplanırken yalnızca aktif Opportunity'lerin tahmini değerleri dikkate alınmalıdır.

Örneğin:

```text
Opportunity A → 100.000 TL → Teklif
Opportunity B → 150.000 TL → Müzakere
Opportunity C → 75.000 TL → Kazanıldı
```

Aktif pipeline değeri:

**100.000 + 150.000 = 250.000 TL**

olarak hesaplanabilir.

Kazanılmış veya kaybedilmiş fırsatlar aktif pipeline değerine dahil edilmemelidir.

---

## 6. Kullanıcı ve Yetki Kuralları

### BR-19 — Sales Representative Yetkisi

Sales Representative:

* Kendi Lead'lerini görüntüleyebilmeli
* Lead bilgilerini güncelleyebilmeli
* Aktivite ekleyebilmeli
* Kendi Opportunity'lerini takip edebilmeli

---

### BR-20 — Sales Manager Yetkisi

Sales Manager, kendi ekibinin:

* Lead'lerini
* Opportunity'lerini
* Pipeline kayıtlarını

görüntüleyebilmelidir.

---

### BR-21 — CRM Administrator Yetkisi

CRM Administrator:

* Kullanıcıları
* Rolleri
* Yetkileri
* Temel CRM tanımlarını

yönetebilmelidir.

---

## 7. Veri Kuralları

### BR-22 — Lead Kaynağı

Her Lead için Lead Kaynağı bilgisi tutulmalıdır.

Örneğin:

* Web sitesi
* Sosyal medya
* Telefon
* E-posta
* Referans
* Etkinlik

---

### BR-23 — Kayıt Kimliği

Lead ve Opportunity kayıtlarının sistem içerisinde benzersiz bir ID'si bulunmalıdır.

Bu ID, kayıtların birbirinden ayırt edilmesini sağlar.

---

### BR-24 — Tarih Bilgileri

Lead ve Opportunity kayıtlarında temel tarih bilgileri tutulmalıdır.

Örneğin:

* Oluşturulma tarihi
* Güncellenme tarihi
* Beklenen kapanış tarihi

---

## 8. Business Rules Özeti

| ID    | Kural                                         | İlgili Alan |
| ----- | --------------------------------------------- | ----------- |
| BR-01 | Lead zorunlu bilgileri                        | Lead        |
| BR-02 | Lead sorumlusu                                | Lead        |
| BR-03 | Lead durumu                                   | Lead        |
| BR-04 | Lead durum güncelleme                         | Lead        |
| BR-05 | Niteliksiz Lead dönüştürülemez                | Lead        |
| BR-06 | Nitelikli Lead dönüştürülebilir               | Lead        |
| BR-07 | Dönüşüm tekrarlanamaz                         | Lead        |
| BR-08 | Aktivite Lead/Opportunity ile ilişkili olmalı | Activity    |
| BR-09 | Aktivite türü bulunmalı                       | Activity    |
| BR-10 | Aktivite tarihi bulunmalı                     | Activity    |
| BR-11 | Opportunity sorumlusu                         | Opportunity |
| BR-12 | Opportunity aşaması                           | Opportunity |
| BR-13 | Aşama geçişleri                               | Opportunity |
| BR-14 | Kazanılan Opportunity kapanır                 | Opportunity |
| BR-15 | Kaybedilen Opportunity'de neden belirtilir    | Opportunity |
| BR-16 | Kapanan Opportunity aktif değildir            | Opportunity |
| BR-17 | Aktif Opportunity pipeline'da görünür         | Pipeline    |
| BR-18 | Pipeline değeri                               | Pipeline    |
| BR-19 | Sales Representative yetkisi                  | User        |
| BR-20 | Sales Manager yetkisi                         | User        |
| BR-21 | CRM Administrator yetkisi                     | User        |
| BR-22 | Lead kaynağı                                  | Lead        |
| BR-23 | Benzersiz kayıt ID'si                         | Data        |
| BR-24 | Tarih bilgileri                               | Data        |

---

## 9. BA Açısından Business Rules

Business Analyst açısından Business Rules'ın amacı, gereksinimlerin yalnızca genel seviyede kalmasını engellemektir.

Örneğin:

**Functional Requirement:**

> Sistem Lead'in Opportunity'ye dönüştürülmesini sağlamalıdır.

Buna karşılık Business Rule:

> Yalnızca Nitelikli durumundaki Lead Opportunity'ye dönüştürülebilir.

Böylece sistem geliştirilirken hangi koşulun uygulanacağı netleşir.

Business Rules ayrıca ilerleyen aşamalarda:

* User Stories
* Acceptance Criteria
* Test Scenarios
* UAT

hazırlanırken kullanılacaktır.
