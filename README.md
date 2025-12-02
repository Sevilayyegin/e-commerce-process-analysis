# 🎯 E-TİCARET BÜYÜME STRATEJİSİ: RFM TABANLI MÜŞTERİ SEGMENTASYONU VE SÜREÇ İYİLEŞTİRME VAKASI

Bu proje, Birleşik Krallık merkezli bir e-ticaret şirketinin 2010-2011 satış verilerini baz alarak kritik **iş sorunlarını** tespit etmek, **müşteri kayıp riskini (Churn)** analiz etmek ve operasyonel verimsizlikleri gidermeye yönelik **somut, eylem odaklı çözümler** önermek amacıyla yürütülmüştür.

Bu çalışma, klasik veri analizinin ötesine geçerek bir **İş Analisti (BA) Yaşam Döngüsünü** uygulamalı olarak göstermektedir: Sorun Tanımlama, Süreç Modelleme (As-Is/To-Be), Çözüm Tasarımı ve İş Değeri Hesaplama.

---

## 📌 İŞ DURUMU (BUSINESS CASE) VE KAPSAM

Harika. Vaka çalışmanızın **"İş Durumu ve Kapsam"** (Business Case & Scope) bölümü, bir İş Analisti'nin projesinin amacını ve değerini üst yönetime net bir şekilde iletmesi açısından hayati önem taşır.

Yaptığımız analizleri ve önerdiğim iyileştirmeleri (uluslararası büyüme odaklı) içerecek şekilde, bu kısmı **profesyonel ve odaklanmış** bir dille yeniden düzenleyelim.

---

## 📌 2. İŞ DURUMU VE PROJE KAPSAMI

Bu proje, mevcut **As-Is** durumundaki kritik iş risklerini tanımlayarak, hedeflenen **To-Be** durumuna ulaşmak için bir yol haritası sunmaktadır.

### 2.1. İş Problemi ve Stratejik Gerekçe (The Business Need)

Şirket, operasyonel ve stratejik düzeyde iki ana zorlukla karşı karşıyadır:

1.  **Tek Pazar Bağımlılığı Riski:** Toplam gelirin %80'den fazlasının Birleşik Krallık'tan gelmesi, şirketi ekonomik ve politik dalgalanmalara karşı savunmasız bırakmaktadır. Uluslararası pazarlardaki **büyüme potansiyeli** yeterince değerlendirilememektedir.
2.  **Yüksek Operasyonel Kayıp:** %9 seviyesindeki iade oranı (yaklaşık £896K parasal karşılığı), lojistik ve paketleme süreçlerinde verimsizlik olduğunu ve müşteri memnuniyetinin düştüğünü göstermektedir. Bu, doğrudan **kar marjını** eriten bir maliyet kalemidir.

### 2.2. Proje Hedefleri ve Kapsam (To-Be Durumu)

Projenin temel hedefi, **RFM segmentasyonunu** kullanarak uluslararası pazarlarda sürdürülebilir bir büyüme sağlamak ve operasyonel maliyetleri düşürmektir.

#### A. Stratejik Hedef (Büyüme ve Elde Tutma)

* **Odak:** Fransa, Almanya, Hollanda, EIRE ve Avustralya pazarları.
* **Amaç:** RFM segmentlerine özel kişiselleştirilmiş kampanyalar ile **kayıp riski** altındaki müşterileri geri kazanmak ve **en değerli (Champions)** müşterilerin sadakatini artırmak.

#### B. Operasyonel Hedef (Süreç İyileştirme)

* **Amaç:** Mevcut **manuel ve yavaş iade sürecini** iyileştirmek için **Self-Servis İade Portalı** çözümü tasarlamak. Bu sayede hem operasyonel maliyetler düşürülecek hem de müşteri deneyimi iyileştirilecektir.

### 2.3. Başarı Kriterleri (Key Performance Indicators - KPIs)

Bu projenin başarısı, aşağıdaki somut ve ölçülebilir iş hedefleri ile değerlendirilecektir:

| Hedeflenen İyileşme Alanı | Mevcut Durum | Hedeflenen KPI |
| :--- | :--- | :--- |
| **Müşteri Geri Kazanım** | At Risk / Lost segmenti varlığı | Yeniden satın alma oranı (Recapture Rate) **%15 artış** |
| **Sadakat Programı Eşiği** | Champions AOV: £257.72 | **Champions** segmentinde Ortalama Sipariş Değerinde (AOV) **%5 artış** sağlanması. |
| **Operasyonel Verimlilik** | İade Oranı: %9 | İade oranını **%7'ye düşürmek** |

## ⚙️ PROJE YÖNETİMİ VE METODOLOJİ

Proje, **Çevik (Agile)** metodoloji ile yürütülmüş, adımlar kısa sprint'lere ayrılmış ve ilerleme **Kanban** yaklaşımıyla takip edilmiştir. 

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
