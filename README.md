# 🎯 E-TİCARET SÜREÇ İYİLEŞTİRME VE CLV OPTİMİZASYON PROJESİ

Bu proje, Birleşik Krallık merkezli bir e-ticaret şirketinin 2010-2011 satış verilerini baz alarak kritik **iş sorunlarını** tespit etmek, **müşteri kayıp riskini (Churn)** analiz etmek ve operasyonel verimsizlikleri gidermeye yönelik **somut, eylem odaklı çözümler** önermek amacıyla yürütülmüştür.

Bu çalışma, klasik veri analizinin ötesine geçerek bir **İş Analisti (BA) Yaşam Döngüsünü** uygulamalı olarak göstermektedir: Sorun Tanımlama, Süreç Modelleme (As-Is/To-Be), Çözüm Tasarımı ve İş Değeri Hesaplama.

---

## 📌 İŞ DURUMU (BUSINESS CASE) VE KAPSAM

### İş Problemi ve Odak Alanı (The Why)

* **Problem:** Müşteri segmentasyonu sonuçları, müşteri tabanının önemli bir kısmının (**At Risk / Lost** ve **Needs Attention** segmentleri) **kayıp riski** altında olduğunu göstermektedir. Ayrıca, **yüksek iade oranı (%9)** müşteri memnuniyetini düşürmekte ve operasyonel maliyetleri artırmaktadır.
* **Proje Hedefi:** Kayıp riski altındaki müşterileri yeniden aktive etmek ve yüksek iade oranına yol açan mevcut süreçlerde **iyileştirme gereksinimlerini** belirlemek.

### Başarı Kriterleri (KPIs)

| Hedeflenen İyileşme Alanı | Mevcut Durum | Hedeflenen KPI |
| :--- | :--- | :--- |
| **Müşteri Sadakati** | At Risk / Lost segmenti varlığı | Yeniden satın alma oranı (Recapture Rate) **%15 artış** |
| **Operasyonel Verimlilik** | İade Oranı: %9 | İade oranını **%7'ye düşürmek** |

---

## ⚙️ PROJE YÖNETİMİ VE METODOLOJİ

Proje, **Çevik (Agile)** metodoloji ile yürütülmüş, adımlar kısa sprint'lere ayrılmış ve ilerleme **Kanban** yaklaşımıyla takip edilmiştir. (Bu aşama, JIRA veya Trello gibi araçlarda görselleştirilebilir.)

| Faz | Ana Odak | Kullanılan BA Aracı/Metodu |
| :--- | :--- | :--- |
| **1. Veri ve Gereksinim** | İş problemini tanımlama ve veri erişimi. | **SQL** (Veri Çekimi), **Scrum** (Sprint Planlama) |
| **2. Mevcut Durum Analizi (AS-IS)** | Kritik iş sürecinin (İade/Geri Kazanım) mevcut durumunu anlama. | **Draw.io / MS Visio** (AS-IS Süreç Modelleme) |
| **3. Çözüm Tasarımı (TO-BE)** | İyileştirme gereksinimlerini belirleme ve çözüm önerme. | **Balsamiq / Mockflow** (Wireframe), **Gereksinim Belirleme** |

---

## 📊 ANA ANALİZ ÇIKTILARI VE İŞ ÇIKARIMLARI

### 1. Müşteri Segmentasyonunun Değerlendirilmesi (RFM)

RFM analizi, stratejik odaklanılması gereken segmentleri netleştirdi:

| Segment | Risk Seviyesi | Önerilen Strateji | Eylem Gereksinimi |
| :--- | :--- | :--- | :--- |
| **Needs Attention** | Orta - Yüksek | Tekrar alışverişi tetiklemek. | Kişiselleştirilmiş e-posta otomasyonu **(Tekrar Etkileşim)** |
| **At Risk / Lost** | Çok Yüksek | Geri kazanım kampanyaları. | İade sürecini hızlandıran **yeni bir self-servis arayüzü**. |
| **Champions** | Düşük | Elde tutma ve sadakati ödüllendirme. | **VIP/Premium** özelliklerin eklenmesi. |

### 2. İade Süreci Kök Neden Analizi

%9'luk iade oranı kritik bir operasyonel sorundur. Analiz, iadelerin yüksek oranda **düşük fiyatlı, yüksek hacimli** ürünlerde toplandığını gösterdi (muhtemel sebepler: paketleme hatası, yanlış ürün bilgisi).

**Sonuç:** Mevcut iade sürecinin **zahmetli** ve **yavaş** olması, kayıp müşterilerin geri kazanılmasını zorlaştırmaktadır.

---

## 🛠️ SÜREÇ İYİLEŞTİRME VE ÇÖZÜM ÖNERİLERİ

### A. Mevcut Durum (AS-IS) Süreç Modellemesi

Müşterinin manuel ve yavaş olan mevcut iade süreci (e-posta/çağrı bekleme, kargoya götürme, uzun geri ödeme süresi) **Draw.io/Visio** ile modellenmiştir.



[Image of a Business Process Flow Diagram]


* **Tespit Edilen Engeller (Pain Points):** Manuel onay adımı, müşteri için kargo zahmeti, geri ödeme süresinin uzunluğu.

### B. Hedef Durum (TO-BE) ve Çözüm Tasarımı

Müşteri kaybını azaltmak ve iade sürecini hızlandırmak için yeni bir **"Self-Servis İade ve Geri Kazanım Portalı"** önerilmiştir.

#### 1. Yeni İş Gereksinimleri (Requirements)

| ID | Gereksinim Tipi | Açıklama | Çözüm Desteği |
| :--- | :--- | :--- | :--- |
| **BR-001** | Fonksiyonel | Müşteri, faturası üzerinden 5 dakikadan kısa sürede iade oluşturabilmelidir. | **TO-BE Süreci** |
| **BR-002** | Fonksiyonel | Kayıp riskli müşterilere iade yerine **anında kredi/kupon** teklif edilmelidir. | **RFM Stratejisi** |
| **NFR-001** | Performans | Geri ödeme süresi 7 iş gününden **48 saate** düşürülmelidir. | **Operasyonel İyileşme** |

#### 2. Self-Servis Arayüz Tasarımı (Balsamiq Wireframe)

Önerilen yeni sürecin ön yüzünü göstermek amacıyla **Balsamiq** (veya eşdeğeri) ile basit bir tel kafes (wireframe) taslağı oluşturulmuştur. Bu taslak, müşterinin hızlıca iade seçeneğini seçmesini ve alternatif olarak bir sonraki alışverişi için anında **hediye çeki** almasını sağlamaktadır.



### C. Hedef Durum (TO-BE) Süreç Modellemesi

Önerilen çözümü içeren, daha hızlı ve verimli olan Hedef Durum süreci **Draw.io/Visio** ile modellenmiştir.

* **İyileşme:** Manuel adımlar ortadan kalkar, müşteriye anında **kredi/kupon** teklif edilerek (kayıp riski altındaki müşteriler için) paranın şirket içinde kalması sağlanır.

---

## 📎 SONUÇ VE İŞ DEĞERİ

Bu proje, veri analizini doğrudan **uygulanabilir iş kararlarına** dönüştürmüştür.

| Öneri | Beklenen İş Etkisi |
| :--- | :--- |
| **Geri Kazanım Kampanyaları** | **At Risk / Lost** segmentlerinin %15'inin geri kazanılmasıyla **XXX TL** gelir artışı. |
| **Self-Servis İade** | Operasyonel maliyetlerin azalması ve müşteri memnuniyetinin artması sonucu **İade Oranında %2 düşüş.** |

Bu çalışma, İş Analisti olarak **problem çözme, paydaşlarla iletişim kurma (model/tasarım) ve veri sonuçlarını iş sonuçlarına çevirme** yeteneğimi göstermektedir.
