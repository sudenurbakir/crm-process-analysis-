# Functional Requirements

## 1. Genel Bakış

Bu doküman, CRM sisteminin Lead ve Opportunity süreçlerini desteklemek için sahip olması gereken fonksiyonel gereksinimleri tanımlar.

Fonksiyonel gereksinimler, sistemin **ne yapması gerektiğini** açıklamaktadır.

---

## 2. Lead Yönetimi

### FR-01 — Lead Oluşturma

Sistem, yetkili kullanıcının yeni bir Lead kaydı oluşturmasına izin vermelidir.

Kullanıcı aşağıdaki bilgileri girebilmelidir:

* Ad Soyad
* Şirket
* E-posta
* Telefon
* Lead Kaynağı
* Sorumlu Satış Temsilcisi

---

### FR-02 — Zorunlu Alan Kontrolü

Sistem, Lead oluşturulurken zorunlu alanların doldurulup doldurulmadığını kontrol etmelidir.

Zorunlu alanlardan biri boş bırakılırsa sistem kullanıcıya hata mesajı göstermeli ve kaydın oluşturulmasına izin vermemelidir.

---

### FR-03 — Lead Listeleme

Sistem, kullanıcıya Lead kayıtlarını listeleyebilmelidir.

Liste üzerinde en az aşağıdaki bilgiler görüntülenmelidir:

* Lead adı
* Şirket
* Lead kaynağı
* Sorumlu kişi
* Lead durumu
* Oluşturulma tarihi

---

### FR-04 — Lead Arama ve Filtreleme

Kullanıcı Lead kayıtlarını aşağıdaki kriterlere göre arayabilmeli veya filtreleyebilmelidir:

* Lead adı
* Şirket
* Lead durumu
* Lead kaynağı
* Sorumlu satış temsilcisi

---

### FR-05 — Lead Güncelleme

Yetkili kullanıcı, mevcut Lead bilgilerinde değişiklik yapabilmelidir.

Değiştirilen bilgiler sistem tarafından güncellenerek kaydedilmelidir.

---

## 3. Lead Durum Yönetimi

### FR-06 — Lead Durumu Güncelleme

Kullanıcı Lead'in durumunu sistem üzerinden değiştirebilmelidir.

Sistem aşağıdaki durumları desteklemelidir:

* Yeni
* İletişime Geçilecek
* İletişim Kuruldu
* Nitelikli
* Niteliksiz
* Dönüştürüldü
* Kayıp

---

### FR-07 — Durum Geçişlerinin Kontrolü

Sistem, Lead durumlarının tanımlanan süreç doğrultusunda güncellenmesini sağlamalıdır.

Örneğin:

**Yeni → İletişime Geçilecek → İletişim Kuruldu → Nitelikli → Dönüştürüldü**

Niteliksiz veya kayıp olarak işaretlenen Lead'ler satış fırsatına dönüştürülmemelidir.

---

## 4. Aktivite Yönetimi

### FR-08 — Aktivite Oluşturma

Kullanıcı bir Lead veya Opportunity için aktivite kaydı oluşturabilmelidir.

Aktivite türleri:

* Telefon
* E-posta
* Toplantı
* Not

olmalıdır.

---

### FR-09 — Aktivite Detayı

Aktivite kaydında aşağıdaki bilgiler tutulmalıdır:

* Aktivite türü
* Tarih
* Açıklama
* İlgili Lead veya Opportunity
* Aktiviteyi oluşturan kullanıcı

---

### FR-10 — Aktivite Görüntüleme

Kullanıcı, ilgili Lead veya Opportunity üzerinde daha önce oluşturulan aktiviteleri görüntüleyebilmelidir.

Aktiviteler tarih sırasına göre listelenebilmelidir.

---

## 5. Lead Değerlendirme ve Dönüşüm

### FR-11 — Lead'i Nitelikli Olarak İşaretleme

Yetkili satış temsilcisi, değerlendirdiği Lead'i **Nitelikli** olarak işaretleyebilmelidir.

---

### FR-12 — Lead'i Niteliksiz Olarak İşaretleme

Yetkili satış temsilcisi, uygun olmayan Lead'i **Niteliksiz** olarak işaretleyebilmelidir.

---

### FR-13 — Lead Dönüştürme

Nitelikli bir Lead için **Opportunity'ye Dönüştür** işlemi yapılabilmelidir.

Dönüştürme işlemi sırasında sistem gerekli müşteri ve fırsat bilgilerinin oluşturulmasını veya mevcut kayıtlarla ilişkilendirilmesini sağlamalıdır.

---

### FR-14 — Dönüştürülen Lead Kontrolü

Dönüştürülmüş bir Lead tekrar Opportunity'ye dönüştürülememelidir.

Sistem kullanıcıya Lead'in daha önce dönüştürüldüğünü belirtmelidir.

---

## 6. Opportunity Yönetimi

### FR-15 — Opportunity Oluşturma

Sistem, yetkili kullanıcının yeni bir Opportunity oluşturmasına izin vermelidir.

Opportunity için aşağıdaki bilgiler girilebilmelidir:

* Opportunity adı
* Müşteri
* Sorumlu satış temsilcisi
* Tahmini değer
* Beklenen kapanış tarihi
* Aşama

---

### FR-16 — Opportunity Listeleme

Kullanıcı mevcut Opportunity kayıtlarını listeleyebilmelidir.

Liste üzerinde en az:

* Opportunity adı
* Müşteri
* Sorumlu kişi
* Aşama
* Tahmini değer
* Beklenen kapanış tarihi

bilgileri görüntülenmelidir.

---

### FR-17 — Opportunity Güncelleme

Yetkili kullanıcı Opportunity bilgilerini güncelleyebilmelidir.

Örneğin:

* Aşama
* Tahmini değer
* Beklenen kapanış tarihi
* Sorumlu kişi

güncellenebilmelidir.

---

## 7. Sales Pipeline

### FR-18 — Opportunity Aşaması Güncelleme

Kullanıcı Opportunity'nin pipeline içerisindeki aşamasını değiştirebilmelidir.

Desteklenen aşamalar:

1. Yeni Fırsat
2. İhtiyaç Analizi
3. Teklif
4. Müzakere
5. Kazanıldı
6. Kaybedildi

---

### FR-19 — Pipeline Görünümü

Sistem, Opportunity'lerin mevcut aşamalarını toplu olarak görüntüleyebilecek bir pipeline görünümü sağlamalıdır.

Kullanıcı hangi Opportunity'nin hangi aşamada olduğunu görebilmelidir.

---

### FR-20 — Kazanılan Opportunity

Opportunity **Kazanıldı** olarak işaretlendiğinde sistem fırsatın satış sürecinin başarıyla tamamlandığını göstermelidir.

---

### FR-21 — Kaybedilen Opportunity

Opportunity **Kaybedildi** olarak işaretlendiğinde sistem kullanıcıdan kayıp nedenini girmesini istemelidir.

---

## 8. Rol ve Yetki Yönetimi

### FR-22 — Kullanıcı Rolleri

Sistem aşağıdaki temel kullanıcı rollerini desteklemelidir:

* Sales Representative
* Sales Manager
* CRM Administrator

---

### FR-23 — Rol Bazlı Erişim

Sistem, kullanıcının rolüne göre erişebileceği kayıtları ve işlemleri kontrol etmelidir.

Örneğin:

**Sales Representative**

* Kendi Lead'lerini görüntüleme
* Lead güncelleme
* Aktivite ekleme
* Opportunity takip etme

**Sales Manager**

* Ekibin Lead'lerini görüntüleme
* Opportunity'leri takip etme
* Pipeline'ı görüntüleme

**CRM Administrator**

* Kullanıcıları yönetme
* Roller ve yetkileri yönetme
* CRM tanımlarını yönetme

---

## 9. Raporlama

### FR-24 — Lead Raporlama

Sistem, Lead kayıtları üzerinden temel raporlar oluşturabilmelidir.

Örneğin:

* Toplam Lead sayısı
* Lead durumlarına göre dağılım
* Lead kaynaklarına göre dağılım
* Sorumlu kişilere göre Lead sayısı

---

### FR-25 — Opportunity Raporlama

Sistem, Opportunity kayıtları üzerinden temel satış raporları oluşturabilmelidir.

Örneğin:

* Toplam Opportunity sayısı
* Pipeline aşamalarına göre Opportunity sayısı
* Kazanılan Opportunity sayısı
* Kaybedilen Opportunity sayısı
* Toplam tahmini Opportunity değeri

---

## 10. Gereksinim Özeti

| ID    | Gereksinim                     | Alan               |
| ----- | ------------------------------ | ------------------ |
| FR-01 | Lead oluşturma                 | Lead               |
| FR-02 | Zorunlu alan kontrolü          | Lead               |
| FR-03 | Lead listeleme                 | Lead               |
| FR-04 | Lead arama ve filtreleme       | Lead               |
| FR-05 | Lead güncelleme                | Lead               |
| FR-06 | Lead durumu güncelleme         | Lead               |
| FR-07 | Durum geçiş kontrolü           | Lead               |
| FR-08 | Aktivite oluşturma             | Activity           |
| FR-09 | Aktivite detayı                | Activity           |
| FR-10 | Aktivite görüntüleme           | Activity           |
| FR-11 | Lead'i nitelikli işaretleme    | Lead               |
| FR-12 | Lead'i niteliksiz işaretleme   | Lead               |
| FR-13 | Lead dönüştürme                | Lead / Opportunity |
| FR-14 | Dönüşüm kontrolü               | Lead               |
| FR-15 | Opportunity oluşturma          | Opportunity        |
| FR-16 | Opportunity listeleme          | Opportunity        |
| FR-17 | Opportunity güncelleme         | Opportunity        |
| FR-18 | Opportunity aşaması güncelleme | Opportunity        |
| FR-19 | Pipeline görünümü              | Opportunity        |
| FR-20 | Kazanılan Opportunity          | Opportunity        |
| FR-21 | Kaybedilen Opportunity         | Opportunity        |
| FR-22 | Kullanıcı rolleri              | User               |
| FR-23 | Rol bazlı erişim               | User               |
| FR-24 | Lead raporlama                 | Reporting          |
| FR-25 | Opportunity raporlama          | Reporting          |

## 11. Sonraki Aşama

Bu fonksiyonel gereksinimler temel alınarak CRM'in Lead ve Opportunity süreçlerinin nasıl çalışacağı detaylandırılacaktır.

Sonraki aşamada **Lead Management** süreci incelenecek ve Lead'in sisteme girişinden değerlendirilmesine kadar olan süreç analiz edilecektir.
