# Sales Pipeline

## 1. Genel Bakış

Sales Pipeline, satış fırsatlarının (Opportunity) satış sürecindeki mevcut durumlarını takip etmek için kullanılan yapıdır.

Bir Lead nitelikli hale gelip Opportunity'ye dönüştürüldükten sonra satış süreci pipeline üzerinden takip edilir.

Temel akış:

**Yeni Fırsat → İhtiyaç Analizi → Teklif → Müzakere → Kazanıldı / Kaybedildi**

---

## 2. Opportunity Nedir?

Opportunity, satışa dönüşme potansiyeli bulunan somut bir satış fırsatıdır.

Örneğin:

Bir şirket CRM yazılımı hakkında bilgi almak için iletişime geçtiğinde bu kayıt başlangıçta **Lead** olabilir.

Satış temsilcisi ihtiyaç olduğunu ve satış potansiyelini doğruladığında:

**Lead → Opportunity**

dönüşümü gerçekleşir.

Örnek:

> Lead: ABC Teknoloji
> İlgilendiği ürün: CRM Yazılımı

↓

> Opportunity: ABC Teknoloji – CRM Lisans Satışı

Artık satış ekibi bu fırsatı pipeline içerisinde takip eder.

---

## 3. Sales Pipeline Aşamaları

Bu projede pipeline aşağıdaki aşamalardan oluşmaktadır:

| Aşama           | Açıklama                           |
| --------------- | ---------------------------------- |
| Yeni Fırsat     | Opportunity yeni oluşturuldu       |
| İhtiyaç Analizi | Müşterinin ihtiyaçları inceleniyor |
| Teklif          | Müşteriye teklif sunuluyor         |
| Müzakere        | Fiyat veya koşullar görüşülüyor    |
| Kazanıldı       | Satış başarıyla tamamlandı         |
| Kaybedildi      | Satış gerçekleşmedi                |

---

## 4. Aşama 1 — Yeni Fırsat

Opportunity oluşturulduğunda başlangıç aşaması **Yeni Fırsat** olur.

Bu aşamada temel bilgiler sisteme girilir:

* Opportunity adı
* Müşteri
* Sorumlu satış temsilcisi
* Tahmini değer
* Beklenen kapanış tarihi

Örnek:

> ABC Teknoloji – CRM Lisans Satışı
> Tahmini değer: 100.000 TL
> Sorumlu: Satış Temsilcisi

---

## 5. Aşama 2 — İhtiyaç Analizi

Bu aşamada satış temsilcisi müşterinin ihtiyaçlarını daha detaylı anlamaya çalışır.

Örneğin:

* Hangi ürüne ihtiyaç duyuluyor?
* Kaç kullanıcı olacak?
* Hangi özellikler gerekli?
* Kullanım amacı nedir?
* Tahmini bütçe nedir?
* Ne zaman satın alma planlanıyor?

Bu aşamadaki görüşmeler CRM üzerinde aktivite olarak kayıt altına alınabilir.

---

## 6. Aşama 3 — Teklif

Müşterinin ihtiyacı belirlendikten sonra teklif hazırlanır.

Opportunity içerisinde teklif sürecine ilişkin bilgiler takip edilebilir.

Örneğin:

* Teklif tarihi
* Teklif tutarı
* Teklif durumu
* Teklif ile ilgili notlar

Bu aşamada Opportunity'nin tahmini değeri güncellenebilir.

---

## 7. Aşama 4 — Müzakere

Müşteri teklifi değerlendirdikten sonra fiyat veya diğer ticari koşullar üzerinde görüşmeler başlayabilir.

Örneğin:

* Fiyat değişikliği
* Kullanıcı sayısı
* Paket içeriği
* İndirim
* Ödeme koşulları

Bu süreçte yapılan görüşmeler CRM üzerinde aktivite olarak tutulabilir.

---

## 8. Aşama 5 — Kazanıldı

Müşteri satın alma kararını verdiğinde Opportunity:

**Kazanıldı**

olarak işaretlenir.

Bu durumda satış süreci tamamlanmış kabul edilir.

Örnek:

```text
ABC Teknoloji
        ↓
Yeni Fırsat
        ↓
İhtiyaç Analizi
        ↓
Teklif
        ↓
Müzakere
        ↓
Kazanıldı
```

Kazanılan Opportunity raporlama süreçlerinde kullanılabilir.

---

## 9. Aşama 6 — Kaybedildi

Satış gerçekleşmediğinde Opportunity:

**Kaybedildi**

olarak işaretlenir.

Sistemin mümkün olduğunca kayıp nedenini de tutması gerekir.

Örnek kayıp nedenleri:

* Fiyat
* Rakip tercih edildi
* Bütçe yetersiz
* İhtiyaç ortadan kalktı
* Zamanlama
* Müşteriye ulaşılamadı
* Diğer

Bu bilgiler daha sonra satış sürecinin analiz edilmesinde kullanılabilir.

---

## 10. Pipeline'da Opportunity Hareketi

Bir Opportunity'nin pipeline içerisindeki hareketi aşağıdaki şekilde düşünülebilir:

```text
                 ┌───────────────┐
                 │  Yeni Fırsat  │
                 └───────┬───────┘
                         ↓
                 ┌───────────────┐
                 │ İhtiyaç Analizi│
                 └───────┬───────┘
                         ↓
                 ┌───────────────┐
                 │     Teklif    │
                 └───────┬───────┘
                         ↓
                 ┌───────────────┐
                 │    Müzakere   │
                 └───────┬───────┘
                    ┌────┴────┐
                    ↓         ↓
             ┌──────────┐ ┌──────────┐
             │Kazanıldı │ │Kaybedildi│
             └──────────┘ └──────────┘
```

---

## 11. Pipeline Görünümü

CRM sistemi Opportunity'leri aşamalarına göre toplu olarak gösterebilir.

Örneğin:

| Yeni Fırsat   | İhtiyaç Analizi | Teklif   | Müzakere |
| ------------- | --------------- | -------- | -------- |
| ABC Teknoloji | XYZ Ltd.        | DEF A.Ş. | KLM A.Ş. |
| MNO Ltd.      | QRS A.Ş.        |          |          |

Bu görünüm sayesinde satış ekibi hangi fırsatların hangi aşamada olduğunu hızlı şekilde görebilir.

---

## 12. Opportunity Değeri

Her Opportunity için tahmini bir satış değeri tutulabilir.

Örneğin:

| Opportunity   | Aşama           | Tahmini Değer |
| ------------- | --------------- | ------------: |
| ABC Teknoloji | Teklif          |    100.000 TL |
| XYZ Ltd.      | Müzakere        |    150.000 TL |
| DEF A.Ş.      | İhtiyaç Analizi |     75.000 TL |

Bu bilgiler pipeline'ın toplam potansiyel değerinin hesaplanmasını sağlar.

Örneğin:

**100.000 + 150.000 + 75.000 = 325.000 TL**

Bu rakam gerçekleşmiş satış değil, pipeline içerisindeki **tahmini fırsat değeridir**.

---

## 13. Pipeline'da Aktivite Takibi

Opportunity ile ilgili yapılan işlemler aktivite olarak kaydedilebilir.

Örneğin:

**22.09.2026 — Telefon**

> Müşteri teklif hakkında geri dönüş yaptı. Fiyat üzerinde görüşme talep edildi.

**24.09.2026 — Toplantı**

> Yeni paket seçenekleri müşteriye sunuldu.

Bu kayıtlar Opportunity'nin geçmişinin takip edilmesini sağlar.

---

## 14. Pipeline Analizi

Business Analyst açısından pipeline yalnızca fırsatların listelendiği bir ekran değildir.

Pipeline üzerinden aşağıdaki sorular analiz edilebilir:

### Süreç

* Opportunity hangi aşamada?
* Hangi fırsatlar uzun süredir aynı aşamada?
* Fırsatların ne kadarı teklif aşamasına ulaşıyor?
* Hangi aşamada kayıplar daha fazla?

### Veri

* Opportunity'nin tahmini değeri nedir?
* Beklenen kapanış tarihi nedir?
* Sorumlu satış temsilcisi kim?
* Kayıp nedeni nedir?

### Raporlama

* Toplam pipeline değeri nedir?
* Kaç Opportunity kazanıldı?
* Kaç Opportunity kaybedildi?
* Hangi kayıp nedenleri daha sık görülüyor?

---

## 15. Lead ve Opportunity Arasındaki Fark

Bu iki kavramın karıştırılmaması önemlidir.

| Lead                               | Opportunity                       |
| ---------------------------------- | --------------------------------- |
| Potansiyel müşteri adayıdır        | Somut satış fırsatıdır            |
| Henüz değerlendirme aşamasındadır  | Satış süreci başlamıştır          |
| Lead Management ile takip edilir   | Sales Pipeline ile takip edilir   |
| Nitelikli veya niteliksiz olabilir | Kazanılabilir veya kaybedilebilir |
| Opportunity'ye dönüşebilir         | Satış sonucuyla kapanır           |

Basit şekilde:

**Lead = "Bu kişi/şirket potansiyel müşteri olabilir."**

**Opportunity = "Bu kişi/şirket için somut bir satış fırsatımız var."**

---

## 16. BA Açısından Sales Pipeline

Business Analyst'in pipeline analizinde cevaplaması gereken temel sorular:

* Opportunity hangi aşamalardan geçecek?
* Her aşamanın giriş koşulu nedir?
* Bir Opportunity hangi durumda sonraki aşamaya geçebilir?
* Hangi kullanıcı aşama değişikliği yapabilir?
* Kaybedilen Opportunity'de hangi bilgiler zorunlu?
* Tahmini değer nasıl hesaplanıyor?
* Beklenen kapanış tarihi nasıl belirleniyor?
* Pipeline hangi raporlarda kullanılacak?
* Bir Opportunity aynı anda iki aşamada bulunabilir mi?

Bu sorular, pipeline sürecinin yalnızca görsel olarak değil, **iş kuralları ve sistem gereksinimleri açısından** da analiz edilmesini sağlar.

---

## 17. Süreç Özeti

```text
Lead
  ↓
Nitelendirme
  ↓
Opportunity
  ↓
Yeni Fırsat
  ↓
İhtiyaç Analizi
  ↓
Teklif
  ↓
Müzakere
  ↓
 ┌──────────────┐
 ↓              ↓
Kazanıldı     Kaybedildi
```

Bu yapı CRM satış sürecinin temel pipeline modelini oluşturmaktadır.
