# Requirements Traceability Matrix

## 1. Amaç

Requirements Traceability Matrix (RTM), gereksinimlerin geliştirme ve test süreci boyunca takip edilmesini sağlar.

Bu projede temel bağlantı:

**Business Requirement → Functional Requirement → User Story → Acceptance Criteria → Test Case → UAT**

---

## 2. Traceability Matrix

| Business Requirement                     | Functional Requirement                  | User Story  | Acceptance Criteria                                       | Test Case    | UAT    |
| ---------------------------------------- | --------------------------------------- | ----------- | --------------------------------------------------------- | ------------ | ------ |
| BR-01 Lead oluşturma                     | FR-01 Lead oluşturma                    | US-01       | Gerekli bilgiler girilerek Lead oluşturulabilmeli         | TC-01, TC-02 | UAT-01 |
| BR-05 Lead durum takibi                  | FR-06/07 Durum güncelleme               | US-05       | Lead durumu güncellenebilmeli                             | TC-03        | -      |
| BR-06 Aktivite takibi                    | FR-08/10 Aktivite oluşturma/görüntüleme | US-06/07    | Aktivite Lead veya Opportunity ile ilişkilendirilebilmeli | TC-04        | UAT-06 |
| BR-08 Lead → Opportunity dönüşümü        | FR-13/14 Dönüşüm                        | US-09       | Sadece Qualified Lead Opportunity'ye dönüştürülebilmeli   | TC-05, TC-06 | UAT-03 |
| BR-09 Opportunity takibi                 | FR-15/17/18                             | US-10/11/12 | Opportunity oluşturulabilmeli ve güncellenebilmeli        | TC-08        | UAT-04 |
| BR-10 Sales Pipeline takibi              | FR-19 Pipeline görüntüleme              | US-13       | Aktif Opportunity'ler Pipeline'da görüntülenebilmeli      | TC-08        | UAT-04 |
| BR-11 Kazanılan/Kaybedilen fırsat takibi | FR-20/21 Won/Lost                       | US-14/15    | Lost durumunda kayıp nedeni girilmeli                     | TC-07        | UAT-05 |

---

## 3. Örnek İzleme

Örneğin:

**BR-08:** Lead'in Opportunity'ye dönüştürülmesi

↓

**FR-13:** Qualified Lead'i Opportunity'ye dönüştürme

↓

**US-09:** Sales Representative olarak Qualified Lead'i Opportunity'ye dönüştürmek istiyorum.

↓

**Acceptance Criteria:** Sadece Qualified durumundaki Lead dönüştürülebilmeli.

↓

**TC-05:** Qualified Lead → Opportunity

↓

**UAT-03:** Kullanıcı Qualified Lead'i Opportunity'ye dönüştürebilmeli.

Bu bağlantı sayesinde bir gereksinimin geliştirme ve test sürecindeki karşılığı takip edilebilir.

---

## 4. BA Açısından Neden Önemli?

RTM sayesinde:

* Gereksinimlerin test edilip edilmediği görülebilir.
* Eksik testler fark edilebilir.
* Gereksinim ile test arasındaki bağlantı korunabilir.
* UAT süreci daha kontrollü yürütülebilir.

**Kısaca:** RTM, "Bu gereksinimin testi yapıldı mı?" sorusuna cevap vermeyi sağlar.
