# Business Requirements

## 1. Genel Bakış

CRM sistemi, potansiyel müşterilerin (Lead) sisteme alınması, takip edilmesi, değerlendirilmesi ve uygun durumlarda satış fırsatına (Opportunity) dönüştürülmesi amacıyla kullanılacaktır.

Sistem; satış ekibinin müşteri adaylarını düzenli şekilde takip etmesini, yapılan görüşme ve aktivitelerin kayıt altına alınmasını ve satış fırsatlarının süreç boyunca izlenmesini sağlayacaktır.

---

## 2. İş Gereksinimleri

### BR-01 — Lead Kaydı Oluşturma

Sistem, potansiyel müşterilerin CRM içerisine Lead olarak kaydedilmesini sağlamalıdır.

Lead kaydında en az aşağıdaki bilgiler bulunmalıdır:

* Ad Soyad
* Şirket
* E-posta
* Telefon
* Lead Kaynağı
* Sorumlu Satış Temsilcisi
* Lead Durumu
* Oluşturulma Tarihi

---

### BR-02 — Lead Bilgilerinin Standartlaştırılması

Lead kayıtlarının belirli ve standart alanlardan oluşması sağlanmalıdır.

Zorunlu alanlar tamamlanmadan Lead kaydı oluşturulmamalıdır.

Bu sayede farklı kaynaklardan gelen müşteri adaylarının bilgilerinin aynı formatta tutulması sağlanacaktır.

---

### BR-03 — Lead Kaynağının Takip Edilmesi

Her Lead'in sisteme hangi kaynaktan geldiği takip edilebilmelidir.

Örnek kaynaklar:

* Web sitesi
* Sosyal medya
* Referans
* Telefon
* E-posta
* Etkinlik

Lead kaynağı bilgisi, ilerleyen süreçte hangi kanalların daha fazla müşteri adayı oluşturduğunun analiz edilmesinde kullanılacaktır.

---

### BR-04 — Lead Sorumlusu Atama

Her Lead için sorumlu bir satış temsilcisi belirlenebilmelidir.

Atanan satış temsilcisi kendi sorumluluğundaki Lead'leri görüntüleyebilmeli ve takip edebilmelidir.

---

### BR-05 — Lead Durumunun Takip Edilmesi

Lead'lerin satış sürecindeki mevcut durumları takip edilebilmelidir.

Örnek durumlar:

* Yeni
* İletişime Geçilecek
* İletişim Kuruldu
* Nitelikli
* Niteliksiz
* Dönüştürüldü
* Kayıp

Lead'in mevcut durumu sistem üzerinden güncellenebilmelidir.

---

### BR-06 — Aktivite Takibi

Lead veya Opportunity ile gerçekleştirilen müşteri etkileşimleri CRM üzerinde kayıt altına alınabilmelidir.

Örnek aktiviteler:

* Telefon görüşmesi
* E-posta
* Toplantı
* Not

Her aktivitenin ilgili kayıtla ilişkilendirilmesi sağlanmalıdır.

---

### BR-07 — Lead Değerlendirme

Satış temsilcisi, Lead'i değerlendirebilmeli ve Lead'in satış fırsatına dönüşmeye uygun olup olmadığını belirleyebilmelidir.

Değerlendirme sonucunda Lead:

* Nitelikli
* Niteliksiz

olarak işaretlenebilmelidir.

---

### BR-08 — Lead'in Opportunity'ye Dönüştürülmesi

Nitelikli bir Lead'in satış fırsatına dönüştürülmesi sağlanmalıdır.

Dönüştürme işlemi sonucunda gerekli müşteri ve fırsat bilgilerinin ilgili CRM kayıtlarıyla ilişkilendirilmesi sağlanmalıdır.

---

### BR-09 — Opportunity Takibi

Oluşturulan satış fırsatları CRM üzerinden takip edilebilmelidir.

Her Opportunity için en az aşağıdaki bilgiler takip edilmelidir:

* Opportunity adı
* İlgili müşteri
* Sorumlu satış temsilcisi
* Aşama
* Tahmini değer
* Oluşturulma tarihi
* Beklenen kapanış tarihi

---

### BR-10 — Sales Pipeline Takibi

Opportunity'lerin satış sürecindeki aşamaları takip edilebilmelidir.

Örnek aşamalar:

1. Yeni Fırsat
2. İhtiyaç Analizi
3. Teklif
4. Müzakere
5. Kazanıldı
6. Kaybedildi

Bu yapı sayesinde satış ekibi devam eden fırsatların hangi aşamada olduğunu görebilmelidir.

---

### BR-11 — Kazanılan ve Kaybedilen Fırsatların Takibi

Sonuçlanan Opportunity'lerin kazanıldı veya kaybedildi olarak işaretlenmesi sağlanmalıdır.

Kaybedilen fırsatlar için mümkün olduğunda kayıp nedeni de kayıt altına alınmalıdır.

Örnek kayıp nedenleri:

* Fiyat
* Rakip tercih edildi
* İhtiyaç ortadan kalktı
* Zamanlama
* Müşteriye ulaşılamadı

---

### BR-12 — Rol Bazlı Erişim

CRM içerisindeki kullanıcıların görevlerine uygun yetkilere sahip olması sağlanmalıdır.

Örneğin:

* Satış temsilcisi kendi sorumluluğundaki kayıtları takip edebilmelidir.
* Satış yöneticisi ekibinin Lead ve Opportunity kayıtlarını görüntüleyebilmelidir.
* CRM yöneticisi kullanıcı ve sistem tanımlarını yönetebilmelidir.

---

### BR-13 — Satış Sürecinin Merkezi Olarak CRM Kullanılması

Lead, Opportunity ve aktivite bilgilerinin farklı dosya, e-posta veya kişisel takip yöntemleri yerine CRM üzerinde merkezi olarak tutulması hedeflenmelidir.

Böylece müşteri adaylarının ve satış fırsatlarının durumuna ilişkin bilgiler tek bir sistem üzerinden takip edilebilecektir.

---

### BR-14 — Satış Sürecinin Raporlanabilir Olması

CRM'de tutulan bilgiler üzerinden temel satış analizlerinin yapılabilmesi sağlanmalıdır.

Örneğin:

* Toplam Lead sayısı
* Lead kaynaklarına göre dağılım
* Lead durumlarına göre dağılım
* Opportunity sayısı
* Kazanılan Opportunity sayısı
* Kaybedilen Opportunity sayısı
* Pipeline'daki toplam fırsat değeri

gibi bilgiler raporlanabilir olmalıdır.

---

## 3. İş Gereksinimlerinin Amacı

Bu gereksinimlerle CRM sisteminin aşağıdaki iş ihtiyaçlarını karşılaması hedeflenmektedir:

* Lead bilgilerinin merkezi olarak tutulması
* Lead'lerin standart şekilde yönetilmesi
* Satış sorumluluklarının belirlenmesi
* Müşteri etkileşimlerinin takip edilmesi
* Nitelikli Lead'lerin Opportunity'ye dönüştürülmesi
* Satış fırsatlarının pipeline üzerinden takip edilmesi
* Kazanılan ve kaybedilen fırsatların analiz edilmesi
* Satış sürecinin raporlanabilir hale getirilmesi

Bu gereksinimler, sonraki aşamada oluşturulacak **Functional Requirements** dokümanının temelini oluşturacaktır.
