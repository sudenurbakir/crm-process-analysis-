# Test Scenarios

## 1. Amaç

CRM sistemindeki temel gereksinimlerin doğru çalışıp çalışmadığını kontrol etmek.

---

## 2. Test Senaryoları

| ID    | Test Senaryosu                                 | Beklenen Sonuç                                      |
| ----- | ---------------------------------------------- | --------------------------------------------------- |
| TC-01 | Geçerli bilgilerle Lead oluşturma              | Lead başarıyla oluşturulmalı                        |
| TC-02 | Zorunlu bilgiler eksik Lead oluşturma          | Sistem uyarı vermeli ve kayıt oluşturmamalı         |
| TC-03 | Lead Status güncelleme                         | Yeni Status başarıyla kaydedilmeli                  |
| TC-04 | Lead'e Activity ekleme                         | Activity ilgili Lead'e kaydedilmeli                 |
| TC-05 | Qualified Lead'i Opportunity'ye dönüştürme     | Opportunity oluşturulmalı                           |
| TC-06 | Unqualified Lead'i Opportunity'ye dönüştürme   | Sistem dönüşüme izin vermemeli                      |
| TC-07 | Opportunity'yi Lost olarak işaretleme          | Loss Reason zorunlu olmalı ve kayıt Lost olmalı     |
| TC-08 | Aktif Opportunity'leri Pipeline'da görüntüleme | Aktif fırsatlar doğru Stage bilgisiyle gösterilmeli |

---

## 3. Örnek Test

### TC-05 — Qualified Lead'i Opportunity'ye Dönüştürme

**Ön koşul:** Lead Status = Qualified

**Adımlar:**

1. Qualified Lead açılır.
2. "Convert to Opportunity" seçilir.
3. İşlem onaylanır.

**Beklenen Sonuç:**

Yeni bir Opportunity oluşturulmalı ve Pipeline içerisinde görüntülenmelidir.

---

## 4. Pozitif ve Negatif Test

Testlerde hem sistemin **doğru çalıştığı** hem de **hatalı işlemleri engellediği** kontrol edilmelidir.

### Pozitif Test

> Qualified Lead → Opportunity oluşturulmalı.

### Negatif Test

> Unqualified Lead → Opportunity oluşturulmamalı.

---

## 5. Test Akışı

```text
Requirement
    ↓
Acceptance Criteria
    ↓
Test Scenario
    ↓
Expected Result
```

Bu yapı sayesinde BA, yazılan gereksinimlerin test edilebilir olup olmadığını kontrol edebilir.
