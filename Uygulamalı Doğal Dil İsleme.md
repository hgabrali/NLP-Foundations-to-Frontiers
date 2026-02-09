# Uygulamalı Doğal Dil İşleme: Ham Metinden Sektörel Analizlere

## 📌 Proje Genel Bakışı
Bu depo (repository), **Doğal Dil İşleme (NLP)** alanında kapsamlı bir teknik kılavuz ve uygulama alanı olarak hizmet vermektedir. Yapılandırılmamış insan dilinin işlenebilir verilere dönüştürülme sürecini; özellikle **Sağlık** ve **Finans** gibi yüksek etkili sektörlere odaklanarak incelemektedir.

---

## 🏗 Temel NLP Görevleri
Bu proje, insan dilini etkili bir şekilde işlemek için gereken birkaç temel mimari görevi uygular ve açıklar:

* **Tokenizasyon ve Normalizasyon**: Makine anlayışını kolaylaştırmak için sürekli metnin ayrık birimlere (tokenlar) bölünmesi ve standartlaştırılması (küçük harfe dönüştürme, lemmatizasyon vb.) süreci.
* **Varlık İsmi Tanıma (NER)**: Metin içindeki kurumlar, kronolojik tarihler veya belirli tıbbi terminoloji gibi kilit varlıkların istatistiksel modeller kullanılarak tanımlanması ve kategorize edilmesi.
* **Duygu Analizi**: Metnin arkasındaki duygusal tonu ve öznel niyeti deşifre etmek ve nicelleştirmek için hesaplamalı dilbilimden yararlanılması.
* **Sözdizimi ve Bağımlılık Ayrıştırma (Dependency Parsing)**: Cümle mantığını anlamak için temel dilbilgisel yapının ve kelimeler arasındaki işlevsel ilişkilerin analiz edilmesi.

---

## 🏥 Sektörel Dönüşümler

### 1. Sağlık
* **Klinik Dokümantasyon**: Yapılandırılmamış doktor notlarından ve klinik raporlardan yapılandırılmış, uygulanabilir veriler çıkarmak için NLP algoritmalarının kullanılması.
* **Tahminleyici Analitik**: Olası sağlık risklerini ve tanısal kalıpları erken aşamada belirlemek için hasta geçmişinin ve boylamsal kayıtların sistematik olarak analiz edilmesi.

### 2. Finans
* **Piyasa Duyarlılığı**: Borsa trendlerini ve oynaklığını tahmin etmek için küresel haber akışlarının ve sosyal medya akışlarının gerçek zamanlı işlenmesi.
* **Risk Yönetimi**: Denetim döngüsünü otomatikleştirmek ve karmaşık finansal raporlarda ve işlem günlüklerinde anormal veya hileli kalıpları belirlemek.

---

## ⚠️ Ham Metin İşlemedeki Zorluklar
Ham ve "işlenmemiş" metinlerle çalışmak önemli teknik engeller içerir. Bu depo, aşağıdakileri hafifletmek için gelişmiş stratejiler sunar:

* **Belirsizlik (Ambiguity)**: Kelimelerin özel dilbilimsel bağlamlarına göre farklı anlamlar taşıdığı durumlarda çok anlamlılık (polysemy) ve eş sesliliğin (homonymy) çözülmesi.
* **Slang ve Gürültü**: Sosyal medyadan veya resmi olmayan iletişim kanallarından toplanan verileri temizlemek için sağlam ön işleme boru hatlarının (pipeline) uygulanması.
* **Yapısal Çeşitlilik**: Çeşitli veri kaynaklarında heterojen belge formatlarını ve standart dışı sözdizimini yönetmek için mühendislik çözümleri üretilmesi.

---

## 🛠 Teknoloji Yığını (Tech Stack)

| Bileşen | Teknoloji |
| :--- | :--- |
| **Programlama Dili** | Python |
| **Temel Kütüphaneler** | Spacy, NLTK, Transformers (Hugging Face), Scikit-learn |
| **Geliştirme Ortamları** | Jupyter Notebooks / VS Code |

---

# Doğal Dil İşleme: Yapılandırılmamış Veriden Stratejik İstihbarata

## 1. Yönetici Özeti
Doğal Dil İşleme (NLP); e-postalar, sosyal medya ve klinik notlardan oluşan yapılandırılmamış verilerin "gürültülü" gerçekliği ile operasyonel iş zekasının stratejik gereksinimleri arasında kritik bir köprü görevi görür **(AWS)**. Kuruluşların devasa hacimlerde metin ve ses verisi ürettiği bir çağda NLP, makinelerin önemli rekabet avantajlarının kilidini açmak için insan dilini yorumlamasına, manipüle etmesine ve kavramasına olanak tanır **(AWS)**.

Modern NLP'nin temel değer önerisi; ham metni, gelişmiş ön işleme boru hatları ve karmaşık belge setleri üzerinde çok adımlı (multi-hop) akıl yürütmeyi sağlayan **Grafik Tabanlı Geri Getirme ile Artırılmış Üretim (GraphRAG)** aracılığıyla yapılandırılmış bilgiye dönüştürme yeteneğinde yatar **(arXiv)**. Kurumsal ölçekli uygulamalar için, özellikle **SAP S/4HANA** gibi karmaşık **Kurumsal Kaynak Planlama (ERP)** ortamlarında GraphRAG, yapılandırma kuralları ve işlemsel bağımlılıklar üzerinde akıl yürütmek için zorunlu hale gelmiştir **(arXiv)**.

Ancak, verimlilik ve doğruluk arasında önemli bir stratejik gerilim mevcuttur. Sağlık ve finans gibi yüksek riskli sektörlerde, **Büyük Dil Modeli (LLM)** tabanlı bilgi grafiği oluşturmanın yüksek hesaplama maliyetleri genellikle engelleyicidir. Araştırmalar, **bağımlılık tabanlı bilgi grafiği oluşturma** gibi "endüstriyel sınıf" alternatiflerin, ölçeklenebilir ve maliyet etkin kalırken LLM odaklı sistemlerin performansının **%94'üne** ulaşabildiğini göstermektedir **(arXiv)**.



---

## 2. NLP Ön İşleme Boru Hattının Temelleri
Metin ön işleme yalnızca bir "temizlik" görevi değildir; model performansını artırmak ve çeşitli veri kümelerinde kelime haznesi boyutunu yönetmek için stratejik bir zorunluluktur **(Scale Events, Meegle)**. Kuruluşlar, ham ve gürültülü metni tutarlı bir formata dönüştürerek, alt akış modellerinin anlamsal paraziti minimize eden yapılandırılmış girdilerle beslenmesini sağlar.

### 🔍 Temel Aşamaların Değerlendirilmesi
* **Segmentasyon**: Bu aşama metni tekil cümlelere böler. Temel teknik zorluk, noktalama işaretlerinin belirsizliğidir; örneğin bir nokta cümle sınırını belirtebileceği gibi "A.Ş." gibi kısaltmalarda da yer alabilir **(Scale Events)**. Buradaki başarısızlık, bağlamı bozan "parçalanmış verilere" yol açar; cümle düzeyindeki birimler sözdizimsel ayrıştırmaya çok daha uygundur ve LLM'lerin performansını artırır **(arXiv)**.
* **Tokenizasyon**: Cümleler "token"lara (tekil kelimeler veya ifadeler) dönüştürülür. Bu, sonraki tüm analizlerin yapı taşıdır; ancak standart boşluk ayırma işlemi genellikle anlamı korumak için özel kurallar gerektiren "don't" gibi yapılarla başarısız olur **(Scale Events)**.
* **Büyük/Küçük Harf Normalizasyonu**: Çoğu NLP yazılımı, tutarlılığı sağlamak için tüm metni küçük harfe dönüştürmeyi tercih eder. Bu, modelin "Apple" (marka) ve "apple" (meyve) kelimelerini yalnızca büyük harf kullanımı nedeniyle farklı varlıklar olarak değerlendirmesini önler **(Scale Events)**.
* **Yazım Denetimi**: Bu adım, yazım hatalarının kelime haznesini zayıflatmasını önler; bu da sınıflandırma ve geri getirme görevlerinde yüksek hatırlama (recall) oranını korumak için gereklidir **(Scale Events)**.

### 🛡️ "Gürültü" Azaltma Katmanı
**Stop-word (Etkisiz Kelime) çıkarma**, belge kategorizasyonu veya duygu analizi gibi görevler için çok az ayırt edici değer sağlayan "ve", "veya", "ise" gibi sık kullanılan kelimelerin filtrelenmesini içerir **(Scale Events, ResearchGate)**.

* **Düşük Kaynaklı Diller**: Hintçe için **LiHiSTO** ve Malayalamca için **LiSTOM** gibi özel kütüphaneler, geri getirme performansını artırmak için geliştirilmiştir **(ResearchGate)**.

### 📊 Karşılaştırmalı Analiz: Gövdeleme (Stemming) ve Lemmatizasyon
Her iki teknik de kelimeleri temel bir forma indirgerken, lemmatizasyon daha gelişmiş ve bağlam farkındalığı olan bir yaklaşım sunar.

| Özellik | Stemming (Kaba Sezgisel) | Lemmatizasyon (Morfolojik Analiz) |
| :--- | :--- | :--- |
| **Hedef** | Temel bir "gövde" bulmak için ekleri kesmek **(Scale Events)**. | Dilbilimsel olarak geçerli "lemma"yı veya sözlük formunu tanımlamak **(Stack Overflow)**. |
| **Doğruluk** | Düşük; kelime olmayan sonuçlar üretebilir (örneğin "caring" -> "car") **(Stack Overflow)**. | Yüksek; geçerli bir kök sağlar (örneğin "caring" -> "care") **(Stack Overflow)**. |
| **Hesaplama Maliyeti** | Düşük; basit kurallar veya arama tabloları kullandığı için daha hızlıdır **(Scale Events)**. | Yüksek; morfolojik analiz ve sözlükler gerektirdiği için daha yavaştır **(Scale Events)**. |
| **Sözcük Türü (POS) Farkındalığı** | Hayır; bağlamdan bağımsız olarak tekil kelimeler üzerinde çalışır **(Stack Overflow)**. | Evet; anlamı belirlemek için Sözcük Türlerini (POS) kullanır **(Stack Overflow)**. |

---

## 3. Yapısal Analiz: Ayrıştırma ve Bilgi Çıkarımı
Stratejik NLP, dilbilgisel ilişkileri anlamak için "Kelime Torbası" (Bag of Words) yaklaşımlarının ötesine geçmeyi gerektirir **(arXiv)**.

### 🏗️ Ayrıştırma Metodolojilerinin Karşılaştırılması
* **Öbek Yapısı Ayrıştırma (Constituency Parsing)**: Metni alt ifadelere veya hiyerarşik segmentlere (İsim Öbekleri, Fiil Öbekleri) ayırır.
* **Bağımlılık Ayrıştırma (Dependency Parsing)**: Kelimeleri ikili üst-bağımlı ilişkilerine göre birbirine bağlar. Örneğin; *"Geliştirici kodu yeniden düzenledi"* cümlesinde "düzenledi" üst (head), "geliştirici" ise öznedir **(arXiv)**.

---

## 4. Problem Alanı: Belirsizlik, Gürültü ve Alana Özgü Jargon
* **Anlamsal Belirsizlik**: "Yüz" (sayı mı yoksa çehre mi?) gibi terimler için Kelime Anlamı Belirginleştirme (WSD) gereklidir **(AWS)**.
* **Dilbilimsel Gürültü**: Dijital iletişimdeki kısaltmaların (örn. "nbr") **Kanonik Temsil**'e (örn. "ne haber") dönüştürülmesi için Metin Normalizasyonu gereklidir **(Scale Events)**.
* **Alana Özgü Jargon**: Matematiksel semboller içeren bilimsel belgeler veya **SAP Özel Kod Taşıma (CCM)** günlükleri işlenirken genel NLP kuralları genellikle yetersiz kalır **(arXiv)**.

---

## 5. Karşılaştırmalı Sektörel Analiz: Sağlık vs. Finans

| Sektör | NLP Odak Alanı | Stratejik Hedefler ve Gereksinimler |
| :--- | :--- | :--- |
| **Sağlık** | Klinik notlar, Elektronik Sağlık Kayıtları (EHR) **(AWS, Shaip)**. | **Hedefler**: Klinik geçmişteki kalıpların çıkarılması yoluyla tahminleyici teşhis. <br> **Zorunluluk**: HIPAA uyumluluğu için hassas veri redaksiyonu. |
| **Finans** | Kazanç raporları, risk bayrakları ve SAP CCM günlükleri **(arXiv, Shaip)**. | **Hedefler**: Alfa üretimi ve risk azaltma. <br> **Zorunluluk**: Karmaşık işlemsel bağımlılıkların haritalanması. |

---

## 6. Gelişmiş Mimariler: GraphRAG ve Uç Birim Dağıtımı (Edge Deployment)
Kurumsal ortamlar, çok adımlı akıl yürütmede geleneksel RAG'ın sınırlamalarını çözmek için **GraphRAG**'a yönelmektedir **(arXiv)**.

### 📱 Uç Birim (Edge) İçin Optimizasyon
NLP'yi kısıtlı kaynaklara sahip mobil veya IoT cihazlarında dağıtmak üç temel teknik gerektirir **(ICMLAS 2025)**:
1.  **Budama (Pruning)**: Bellek taleplerini düşürmek için gereksiz parametrelerin elenmesi.
2.  **Nicemleme (Quantization)**: Hesaplama yükünü azaltmak için hassasiyetin düşürülmesi (örn. 32-bit'ten 8-bit'e).
3.  **Bilgi Damıtma (Knowledge Distillation)**: "Öğrenci" modellerin "öğretmen" modelleri taklit edecek şekilde eğitilmesi.

---

## 7. Gelecek Eğilimler ve Etik Hususlar
NLP pazarı 2025 yılına kadar **39,37 milyar dolar** değerine ulaşma yolunda hızla ilerlemektedir **(Shaip)**. 

* **Duygusal Zeka**: Sadece duyguyu değil; hayal kırıklığı, neşe veya alaycılık gibi karmaşık durumları tespit etme.
* **Etik Zorunluluk**: Halüsinasyonları ve algoritmik yanlılığı azaltmak için eğitim verisi kaynaklarını açıklama zorunluluğunun artması.

### 🎯 Sonuç
Doğal Dil İşleme, temel metin temizliğinden 2025 **"Yapay Zeka Çağı"**nın temel motoruna evrilerek insan dünyasının karmaşık ve yapılandırılmış bir şekilde anlaşılmasını sağlamaktadır.

---

# 📊 Bag of Words (BoW) ve TF-IDF: Teknik Karşılaştırma

| Özellik | Bag of Words (BoW) | TF-IDF |
| :--- | :--- | :--- |
| **Kelime Frekansı** | Vektör temsili için ham kelime sayılarını kullanır. | Ters belge frekansı ile düzeltilmiş terim frekansını kullanır. |
| **Kelime Sırası** | Kelime sırasını ve metin içindeki mekansal ilişkileri ihmal eder. | Kelime sırasını ve metin içindeki mekansal ilişkileri ihmal eder. |
| **Odak** | Kelimelerin tekil bir belgedeki ham oluşumuna odaklanır. | Kelimelerin daha geniş bir derlem (corpus) içindeki istatistiksel önemine odaklanır. |
| **Yaygın Kelimelerin Yönetimi** | "ve", "bir" gibi ayırt edici olmayan kelimelere eşit ağırlık verir. | Yaygın "gürültü" kelimelerinin ağırlığını düşürür ve nadir, anlamlı kelimeleri öne çıkarır. |
| **Kullanım Durumu** | Ham frekansın birincil metrik olduğu temel metin analizi görevleri için idealdir. | Arama motoru indeksleme gibi gelişmiş önem sıralaması gerektiren görevlerde üstündür. |

---

# Teknik Karşılaştırmalı Analiz: Temel NLP Metodolojileri

## 📊 Metodoloji Değerlendirme Matrisi

| NLP Kavramı | Teknik Hedef | Temel Farklar ve Karşılaştırmalı Analiz | Hesaplamalı Fayda |
| :--- | :--- | :--- | :--- |
| **Tokenizasyon** | **Metnin Atomizasyonu**: Dizelerin kelime veya cümle gibi ayrık birimlere bölünmesi. | Normalizasyonun aksine karakterleri değiştirmez; sadece verinin yapısal sınırlarını tanımlar. | Tüm alt akış görevleri (NER, Parsing vb.) için zorunlu ilk adım. |
| **Lemmatizasyon** | **Morfolojik İndirgeme**: Kelimelerin geçerli sözlük formuna (lemma) dönüştürülmesi. | Sözlük tabanlıdır. Stemming'den farklı olarak çıktının gerçek bir kelime olmasını sağlar. | Anlamsal bütünlüğün korunması gereken (örn. Soru-Cevap) görevler için kritiktir. |
| **Stop Word Çıkarma** | **Gürültü Filtreleme**: Yüksek frekanslı, düşük bilgili kelimelerin (örn. "ve", "ile") elenmesi. | Anlamsal yoğunluğa odaklanır. Modelin odak noktasını önemli anahtar kelimeler üzerinde toplar. | Öznitelik alanı boyutunu azaltır ve model verimliliğini artırır. |
| **TF-IDF Vektörizasyonu** | **İstatistiksel Ağırlıklandırma**: Belirli bir belgede sık, ancak derlemde nadir olan kelimelerin vurgulanması. | Bilgi değerini frekansın önüne koyar. Tüm belgelerde görünen yaygın kelimeleri cezalandırır. | Bilgi Geri Getirme ve benzersiz belge "imzalarını" tanımlamak için idealdir. |

## 🧠 Uygulama İçin Stratejik Özet
* **Hassasiyet Odaklı Görevler İçin (Sağlık/Hukuk):** Terminoloji bütünlüğünü korumak için Stemming yerine **Lemmatizasyon**'u tercih edin.
* **Performans Odaklı Görevler İçin (Gerçek Zamanlı Analitik):** Gecikmeyi azaltmak için **Stemming** ve agresif **Stop Word Çıkarma** yöntemlerini kullanın.
* **Öznitelik Mühendisliği İçin:** Veri kümesi küçükse, **TF-IDF** genellikle Bag of Words'ten daha üstündür çünkü modele bağlamı tanımlayan "sinyaller" sağlar.
