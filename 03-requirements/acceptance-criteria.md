# Acceptance Criteria

## 1. Amaç

Bu doküman, CRM sistemindeki User Story'lerin tamamlanmış sayılabilmesi için karşılanması gereken koşulları tanımlar.

Acceptance Criteria, bir gereksinimin **hangi şartlarda doğru kabul edileceğini** belirtir.

Temel amaç:

* Gereksinimin netleştirilmesi
* Geliştirici ekibin ne yapacağını anlaması
* Test senaryolarının oluşturulabilmesi
* User Story'nin tamamlanıp tamamlanmadığının kontrol edilmesi

---

# 2. Acceptance Criteria

## US-01 — Lead Oluşturma

**User Story:**
Sales Representative olarak yeni bir Lead oluşturmak istiyorum, böylece potansiyel müşteriyi CRM üzerinde takip edebileyim.

### Acceptance Criteria

* Lead oluşturma ekranı açılabilmelidir.
* Lead Name bilgisi girilebilmelidir.
* Company bilgisi girilebilmelidir.
* Email veya Phone bilgilerinden en az biri girilmelidir.
* Lead Source seçilebilmelidir.
* Owner atanabilmelidir.
* Zorunlu bilgiler eksikse Lead oluşturulmamalıdır.
* Başarılı oluşturulan Lead benzersiz bir Lead ID'ye sahip olmalıdır.

---

## US-02 — Lead Listesini Görüntüleme

**User Story:**
Sales Representative olarak Lead kayıtlarını liste halinde görüntülemek istiyorum.

### Acceptance Criteria

* Kullanıcı Lead listesini açabilmelidir.
* Lead ID görüntülenebilmelidir.
* Lead Name görüntülenebilmelidir.
* Company görüntülenebilmelidir.
* Lead Source görüntülenebilmelidir.
* Owner görüntülenebilmelidir.
* Lead Status görüntülenebilmelidir.
* Oluşturulma tarihi görüntülenebilmelidir.

---

## US-03 — Lead Arama ve Filtreleme

**User Story:**
Sales Representative olarak Lead kayıtlarını aramak ve filtrelemek istiyorum.

### Acceptance Criteria

* Lead Name ile arama yapılabilmelidir.
* Company ile arama yapılabilmelidir.
* Lead Status'a göre filtreleme yapılabilmelidir.
* Lead Source'a göre filtreleme yapılabilmelidir.
* Owner'a göre filtreleme yapılabilmelidir.
* Arama sonucunda kriterlere uyan kayıtlar gösterilmelidir.
* Kriterlere uyan kayıt yoksa kullanıcıya uygun bir bilgi gösterilmelidir.

---

## US-04 — Lead Atama

**User Story:**
Sales Manager olarak Lead kaydını bir Sales Representative'a atamak istiyorum.

### Acceptance Criteria

* Sales Manager Lead kaydını seçebilmelidir.
* Lead için aktif Sales Representative listesi görüntülenmelidir.
* Bir Sales Representative seçilebilmelidir.
* Atama tamamlandığında Lead'in Owner bilgisi güncellenmelidir.
* Her Lead'in bir Owner'ı bulunmalıdır.

---

## US-05 — Lead Durumunu Güncelleme

**User Story:**
Sales Representative olarak Lead durumunu güncellemek istiyorum.

### Acceptance Criteria

* Kullanıcı Lead Status alanını güncelleyebilmelidir.
* Kullanılabilir durumlar sistemde tanımlı olmalıdır.
* Lead aynı anda yalnızca bir aktif statüye sahip olmalıdır.
* Durum değişikliği Lead kaydına yansıtılmalıdır.
* Converted veya Lost gibi kapatılmış durumdaki Lead tekrar aktif hale getirilememelidir.

---

## US-06 — Aktivite Ekleme

**User Story:**
Sales Representative olarak Lead veya Opportunity üzerine aktivite eklemek istiyorum.

### Acceptance Criteria

* Kullanıcı Lead veya Opportunity seçebilmelidir.
* Aktivite türü seçilebilmelidir.
* Aktivite türleri Phone, Email, Meeting ve Note olmalıdır.
* Aktivite tarihi girilmelidir.
* Aktivite açıklaması girilebilmelidir.
* Aktivite ilgili Lead veya Opportunity ile ilişkilendirilmelidir.

---

## US-07 — Aktivite Geçmişini Görüntüleme

**User Story:**
Sales Representative olarak Lead veya Opportunity ile ilgili geçmiş aktiviteleri görüntülemek istiyorum.

### Acceptance Criteria

* Kullanıcı ilgili Lead veya Opportunity'yi açabilmelidir.
* İlgili aktiviteler görüntülenebilmelidir.
* Aktivite türü görüntülenebilmelidir.
* Aktivite tarihi görüntülenebilmelidir.
* Aktivite açıklaması görüntülenebilmelidir.
* Aktiviteler tarih sırasına göre görüntülenebilmelidir.

---

## US-08 — Lead'i Qualified Olarak İşaretleme

**User Story:**
Sales Representative olarak değerlendirmesi tamamlanan Lead'i Qualified olarak işaretlemek istiyorum.

### Acceptance Criteria

* Kullanıcı Lead durumunu Qualified olarak değiştirebilmelidir.
* Lead'in temel bilgilerinin tamamlanmış olması kontrol edilmelidir.
* Qualified olarak işaretlenen Lead satış fırsatına dönüştürülebilmelidir.
* Qualified olmayan Lead doğrudan Opportunity'ye dönüştürülememelidir.

---

## US-09 — Lead'i Opportunity'ye Dönüştürme

**User Story:**
Sales Representative olarak Qualified Lead'i Opportunity'ye dönüştürmek istiyorum.

### Acceptance Criteria

* Yalnızca Qualified Lead dönüştürülebilmelidir.
* Unqualified Lead dönüştürülememelidir.
* Dönüşüm sırasında Opportunity oluşturulabilmelidir.
* Opportunity bir Owner'a sahip olmalıdır.
* Dönüştürülmüş Lead tekrar Opportunity'ye dönüştürülememelidir.
* Oluşturulan Opportunity pipeline içerisinde görüntülenebilmelidir.

---

## US-10 — Opportunity Oluşturma

**User Story:**
Sales Representative olarak yeni bir Opportunity oluşturmak istiyorum.

### Acceptance Criteria

* Opportunity oluşturma ekranı açılabilmelidir.
* Opportunity adı girilebilmelidir.
* İlgili müşteri bilgisi seçilebilmelidir.
* Tahmini değer girilebilmelidir.
* Owner atanabilmelidir.
* Opportunity başlangıç aşaması New Opportunity olmalıdır.
* Opportunity benzersiz bir Opportunity ID'ye sahip olmalıdır.

---

## US-11 — Opportunity Bilgilerini Güncelleme

**User Story:**
Sales Representative olarak Opportunity bilgilerini güncellemek istiyorum.

### Acceptance Criteria

* Kullanıcı Opportunity kaydını açabilmelidir.
* Güncellenebilir bilgiler görüntülenmelidir.
* Tahmini değer güncellenebilmelidir.
* Beklenen kapanış tarihi güncellenebilmelidir.
* Owner bilgisi güncellenebilmelidir.
* Yapılan değişiklikler Opportunity kaydına kaydedilmelidir.

---

## US-12 — Opportunity Stage Güncelleme

**User Story:**
Sales Representative olarak Opportunity'nin satış aşamasını güncellemek istiyorum.

### Acceptance Criteria

* Opportunity'nin mevcut Stage bilgisi görüntülenmelidir.
* Kullanıcı uygun bir sonraki aşamaya geçebilmelidir.
* Aşamalar şu sırayı takip etmelidir:

`New Opportunity → Needs Analysis → Proposal → Negotiation → Won/Lost`

* Won veya Lost durumuna geçen Opportunity kapalı olarak kabul edilmelidir.
* Kapalı Opportunity tekrar aktif aşamaya alınamamalıdır.

---

## US-13 — Sales Pipeline Görüntüleme

**User Story:**
Sales Representative olarak aktif Opportunity kayıtlarını pipeline üzerinde görüntülemek istiyorum.

### Acceptance Criteria

* Aktif Opportunity kayıtları pipeline üzerinde görüntülenebilmelidir.
* Opportunity'nin mevcut Stage bilgisi görüntülenmelidir.
* Opportunity Owner bilgisi görüntülenebilmelidir.
* Tahmini Opportunity değeri görüntülenebilmelidir.
* Won ve Lost Opportunity'ler aktif pipeline içerisinde gösterilmemelidir.
* Aktif Opportunity'lerin toplam tahmini değeri hesaplanabilmelidir.

---

## US-14 — Opportunity'yi Won Olarak İşaretleme

**User Story:**
Sales Representative olarak başarıyla tamamlanan Opportunity'yi Won olarak işaretlemek istiyorum.

### Acceptance Criteria

* Opportunity Negotiation aşamasından Won durumuna geçirilebilmelidir.
* Won durumundaki Opportunity kapalı olarak kabul edilmelidir.
* Won Opportunity aktif pipeline değerine dahil edilmemelidir.
* Won Opportunity tekrar aktif bir aşamaya geçirilememelidir.

---

## US-15 — Opportunity'yi Lost Olarak İşaretleme

**User Story:**
Sales Representative olarak sonuçlanmayan Opportunity'yi Lost olarak işaretlemek istiyorum.

### Acceptance Criteria

* Opportunity Lost olarak işaretlenebilmelidir.
* Lost işlemi sırasında kayıp nedeni seçilmelidir.
* Kayıp nedenleri sistemde tanımlı olmalıdır.
* Kayıp nedenleri arasında Price, Competitor, Budget, Timing ve Need Disappeared bulunmalıdır.
* Lost Opportunity aktif pipeline değerine dahil edilmemelidir.
* Lost Opportunity kapalı olarak kabul edilmelidir.

---

## US-16 — Ekip Pipeline'ını Görüntüleme

**User Story:**
Sales Manager olarak ekibime ait Lead, Opportunity ve pipeline bilgilerini görüntülemek istiyorum.

### Acceptance Criteria

* Sales Manager ekip Lead kayıtlarını görüntüleyebilmelidir.
* Sales Manager ekip Opportunity kayıtlarını görüntüleyebilmelidir.
* Sales Manager ekip pipeline'ını görüntüleyebilmelidir.
* Opportunity'lerin Stage bilgileri görüntülenebilmelidir.
* Opportunity'lerin Owner bilgileri görüntülenebilmelidir.
* Aktif pipeline toplam değeri görüntülenebilmelidir.

---

## US-17 — Kullanıcı ve Rollerini Yönetme

**User Story:**
CRM Administrator olarak CRM kullanıcılarını ve rollerini yönetmek istiyorum.

### Acceptance Criteria

* CRM Administrator kullanıcı listesine erişebilmelidir.
* Yeni kullanıcı oluşturulabilmelidir.
* Kullanıcıya rol atanabilmelidir.
* Kullanıcının aktif/pasif durumu yönetilebilmelidir.
* Kullanıcıların erişimleri rollerine göre kontrol edilmelidir.
* Sales Representative, Sales Manager ve CRM Administrator rolleri tanımlı olmalıdır.

---

## US-18 — Lead Kaynaklarını Görüntüleme

**User Story:**
Sales Manager olarak Lead kayıtlarının hangi kaynaklardan geldiğini görüntülemek istiyorum.

### Acceptance Criteria

* Lead Source bilgisi Lead kayıtlarında tutulmalıdır.
* Kullanıcı Lead Source'a göre filtreleme yapabilmelidir.
* Lead kaynaklarının sayısı görüntülenebilmelidir.
* Kaynak bazında Lead kayıtları karşılaştırılabilmelidir.

---

## US-19 — Opportunity Raporlarını Görüntüleme

**User Story:**
Sales Manager olarak Opportunity sonuçlarını ve pipeline bilgilerini rapor olarak görüntülemek istiyorum.

### Acceptance Criteria

* Aktif Opportunity sayısı görüntülenebilmelidir.
* Won Opportunity sayısı görüntülenebilmelidir.
* Lost Opportunity sayısı görüntülenebilmelidir.
* Aktif pipeline toplam değeri görüntülenebilmelidir.
* Lost Opportunity kayıtlarının kayıp nedenleri görüntülenebilmelidir.
* Raporlar güncel CRM verileri üzerinden oluşturulmalıdır.

---

# 3. Acceptance Criteria Özeti

| User Story | Ana Kabul Kriteri                                |
| ---------- | ------------------------------------------------ |
| US-01      | Geçerli bilgilerle Lead oluşturulabilmeli        |
| US-02      | Lead kayıtları görüntülenebilmeli                |
| US-03      | Lead aranıp filtrelenebilmeli                    |
| US-04      | Lead bir Sales Representative'a atanabilmeli     |
| US-05      | Lead Status güncellenebilmeli                    |
| US-06      | Aktivite eklenebilmeli                           |
| US-07      | Aktivite geçmişi görüntülenebilmeli              |
| US-08      | Lead Qualified olarak işaretlenebilmeli          |
| US-09      | Qualified Lead Opportunity'ye dönüştürülebilmeli |
| US-10      | Opportunity oluşturulabilmeli                    |
| US-11      | Opportunity bilgileri güncellenebilmeli          |
| US-12      | Opportunity Stage güncellenebilmeli              |
| US-13      | Pipeline görüntülenebilmeli                      |
| US-14      | Opportunity Won olarak kapatılabilmeli           |
| US-15      | Opportunity Lost olarak kapatılabilmeli          |
| US-16      | Sales Manager ekip pipeline'ını görebilmeli      |
| US-17      | CRM kullanıcıları ve rolleri yönetilebilmeli     |
| US-18      | Lead kaynakları analiz edilebilmeli              |
| US-19      | Opportunity raporları görüntülenebilmeli         |

---

# 4. BA Açısından Acceptance Criteria

Acceptance Criteria, User Story'nin **“tamamlandı”** kabul edilmesi için gereken şartlardır.

Örneğin:

**User Story:**

> Sales Representative olarak Qualified Lead'i Opportunity'ye dönüştürmek istiyorum.

Acceptance Criteria:

* Yalnızca Qualified Lead dönüştürülebilmeli.
* Unqualified Lead dönüştürülememeli.
* Opportunity oluşturulabilmeli.
* Lead tekrar dönüştürülememeli.

Böylece geliştirici ekip **neyi yapacağını**, BA **hangi koşulların karşılanması gerektiğini**, QA/Test ekibi ise **neyi test edeceğini** daha net görebilir.

Bu proje içerisinde bir sonraki aşamada bu Acceptance Criteria'lar üzerinden **Test Scenarios** oluşturulacaktır.
