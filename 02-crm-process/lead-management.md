# Lead Management

## 1. Genel Bakış

Lead, şirketin ürün veya hizmetleriyle ilgilenme potansiyeli bulunan ancak henüz satış fırsatına dönüşmemiş kişi veya kurum kaydıdır.

CRM sürecinde Lead'in temel amacı, potansiyel müşteriyi kayıt altına almak, değerlendirmek, takip etmek ve uygun olduğunda bir **Opportunity**'ye dönüştürmektir.

Temel süreç:

**Lead Oluşturma → Atama → İlk Değerlendirme → İletişim → Nitelendirme → Dönüşüm / Kayıp**

---

## 2. Lead Nasıl Oluşur?

Lead farklı kanallardan CRM sistemine ulaşabilir.

Örnek kaynaklar:

* Web sitesi
* Sosyal medya
* Telefon
* E-posta
* Referans
* Etkinlik

Örneğin bir potansiyel müşteri web sitesindeki iletişim formunu doldurursa bu kişi CRM içerisinde Lead olarak oluşturulabilir.

---

## 3. Lead Oluşturma

Yeni Lead oluşturulurken temel müşteri adayı bilgileri sisteme girilir.

### Lead Bilgileri

| Alan               | Açıklama                              |
| ------------------ | ------------------------------------- |
| Lead ID            | Lead'in sistemdeki benzersiz numarası |
| Ad Soyad           | Potansiyel müşterinin adı             |
| Şirket             | Bağlı olduğu şirket                   |
| E-posta            | İletişim e-posta adresi               |
| Telefon            | İletişim telefonu                     |
| Lead Kaynağı       | Lead'in geldiği kanal                 |
| Sorumlu            | Lead'den sorumlu satış temsilcisi     |
| Lead Durumu        | Lead'in mevcut durumu                 |
| Oluşturulma Tarihi | Lead'in sisteme giriş tarihi          |

---

## 4. Lead Atama

Lead oluşturulduktan sonra sorumlu satış temsilcisine atanır.

Atama manuel veya sistem tarafından belirlenen kurallara göre otomatik yapılabilir.

Bu projede temel senaryo:

**Lead → Sales Representative**

şeklindedir.

Atama sonrasında satış temsilcisi kendi sorumluluğundaki Lead'i görüntüleyebilir ve takip edebilir.

---

## 5. Lead'in İlk Değerlendirilmesi

Satış temsilcisi Lead kaydını inceleyerek müşteri adayı hakkında mevcut bilgileri kontrol eder.

Kontrol edilebilecek bilgiler:

* İletişim bilgilerinin yeterliliği
* Şirket bilgisi
* İhtiyaç bilgisi
* Lead kaynağı
* Daha önce iletişim kurulup kurulmadığı
* Potansiyel satış ihtimali

Eksik bilgi bulunuyorsa Lead üzerinde gerekli güncellemeler yapılabilir.

---

## 6. Lead ile İletişim

Satış temsilcisi Lead ile iletişime geçer.

İletişim sonucunda yapılan işlem CRM üzerinde aktivite olarak kaydedilir.

Örneğin:

**Aktivite Türü:** Telefon
**Tarih:** 22.09.2026
**Açıklama:** Ürün hakkında bilgi almak istediğini belirtti. Görüşme sonrası teklif talebi değerlendirilecek.

Bu kayıt sayesinde Lead ile daha önce neler yapıldığı takip edilebilir.

---

## 7. Lead Durumlarının Değişimi

Lead'in durumu süreç içerisinde değişebilir.

Örnek akış:

**Yeni**
↓
**İletişime Geçilecek**
↓
**İletişim Kuruldu**
↓
**Nitelikli**

Bu noktadan sonra Lead'in sonucu iki farklı şekilde ilerleyebilir:

### Senaryo 1 — Nitelikli Lead

Lead satış potansiyeline sahipse:

**Nitelikli → Dönüştürüldü → Opportunity**

### Senaryo 2 — Niteliksiz Lead

Satış potansiyeli bulunmuyorsa:

**Nitelikli Değil → Niteliksiz / Kayıp**

---

## 8. Lead Nitelendirme

Lead'in satış fırsatına dönüşmeye uygun olup olmadığı değerlendirilir.

Basit değerlendirme kriterleri:

* Gerçek bir ihtiyaç bulunuyor mu?
* Ürün veya hizmetle ilgileniyor mu?
* İletişim kurulabiliyor mu?
* Potansiyel satın alma ihtimali bulunuyor mu?
* Satış sürecinin devam etmesi anlamlı mı?

Bu değerlendirme sonucunda Lead:

**Nitelikli**

veya

**Niteliksiz**

olarak işaretlenebilir.

---

## 9. Lead'in Opportunity'ye Dönüştürülmesi

Lead nitelikli olarak değerlendirildiğinde satış fırsatına dönüştürülebilir.

Örnek:

**Lead**

> ABC Teknoloji
> Ürün hakkında bilgi almak istiyor.

↓

**Nitelikli Lead**

> İhtiyaç doğrulandı.
> Satış potansiyeli mevcut.

↓

**Opportunity**

> ABC Teknoloji – CRM Lisans Satışı

Opportunity oluşturulduktan sonra satış süreci artık Lead üzerinden değil, Opportunity üzerinden takip edilir.

---

## 10. Lead'in Kayıp Olması

Her Lead satış fırsatına dönüşmeyebilir.

Örneğin:

* Müşteri ürünü istemiyor.
* İhtiyaç bulunmuyor.
* Rakip ürün tercih edildi.
* Müşteriye ulaşılamıyor.
* Satın alma planı bulunmuyor.

Bu durumda Lead uygun bir sonuçla kapatılabilir.

Kayıp nedeni mümkün olduğunca kayıt altına alınmalıdır.

---

## 11. Lead Management Sürecinin Özeti

```text
Lead Kaynağı
     ↓
Lead Oluşturma
     ↓
Lead Atama
     ↓
İlk Değerlendirme
     ↓
İletişim
     ↓
Lead Nitelendirme
     ↓
 ┌───────────────┐
 │               │
Nitelikli      Niteliksiz
 │               │
 ↓               ↓
Opportunity     Kayıp
 │
 ↓
Sales Pipeline
```

---

## 12. BA Açısından Lead Management

Bir Business Analyst için Lead Management sürecinin analizinde aşağıdaki sorular önemlidir:

### İş Süreci

* Lead nasıl oluşuyor?
* Lead'i kim oluşturuyor?
* Lead kime atanıyor?
* Lead hangi aşamalardan geçiyor?
* Hangi durumda Lead nitelikli kabul ediliyor?
* Hangi durumda Lead kaybediliyor?

### Sistem

* Hangi alanlar zorunlu?
* Lead hangi kullanıcılar tarafından görüntülenebilir?
* Lead durumu nasıl değiştiriliyor?
* Hangi aktiviteler kaydediliyor?
* Lead ne zaman Opportunity'ye dönüşebiliyor?

### Veri

* Lead kaynağı tutuluyor mu?
* Sorumlu satış temsilcisi tutuluyor mu?
* Aktivite geçmişi saklanıyor mu?
* Kayıp nedeni kaydediliyor mu?

### Raporlama

* Hangi kaynaktan kaç Lead geliyor?
* Kaç Lead nitelikli oluyor?
* Kaç Lead Opportunity'ye dönüşüyor?
* Kaç Lead kaybediliyor?

Bu sorular, Business Analyst'in yalnızca sistemi değil, sistemin arkasındaki **iş sürecini** anlamasını sağlar.
