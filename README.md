# Prompt Engineering Course

## 📌 Prompt Engineering Temel İlkeleri

| İlke | Açıklama | Örnek (Yanlış ❌ / Doğru ✅) |
|------|----------|-----------------------------|
| **1. Clarity & Specificity (Açıklık ve Belirginlik)** | Sorular net ve belirgin olmalı. Belirsiz sorular geniş/ilgisiz cevaplar doğurur. | ❌ “Python hakkında bilgi ver.” <br> ✅ “Python’da `for` döngüsü ile 1’den 10’a kadar sayıları yazdıran bir örnek kod ver.” |
| **2. Contextual Information (Bağlam Bilgisi)** | Soruna gerekli arka plan bilgilerini ekle. Bu, AI’nın doğru açıdan cevap vermesini sağlar. | ❌ “Bir veritabanı sorgusu yaz.” <br> ✅ “PostgreSQL’de `users` tablosundan aktif kullanıcıların ad ve e-postalarını getiren sorguyu yaz.” |
| **3. Purpose & Goal Orientation (Amaç ve Hedef Odaklılık)** | Amacını açıkça belirt (bilgi almak, problem çözmek, yaratıcı içerik, vb.). | ❌ “Bir şiir yaz.” <br> ✅ “İlkbaharın gelişini anlatan, 4 kıtalık, uyaklı bir şiir yaz.” |
| **4. Structured Approach (Yapılandırılmış Yaklaşım)** | Soruları düzenli bir çerçeveyle sor (liste, adım adım, şablon). | ✅ “Python’da web scraping için: <br> 1. Kullanılacak kütüphaneleri listele. <br> 2. Basit bir örnek kod yaz. <br> 3. En sık karşılaşılan hataları açıkla.” |
| **5. Iterative Refinement (Adım Adım İyileştirme)** | İlk cevaptan sonra sorunu yeniden düzenle, daha fazla detay iste. | İlk: “Bana yapay zekâ hakkında bilgi ver.” <br> Sonra: “Peki, sağlık alanındaki kullanımına örnek ver.” <br> Daha sonra: “Bu örneği Türkiye’deki uygulamalarla ilişkilendir.” |

## 📌 Prompt Engineering Best Practices – Quick Reference

Below is a quick reference table summarizing the best practices in prompt engineering for effective interactions with AI models.

| # | İlke | Kısa Açıklama | Örnek (Daha Etkili ✅ / Daha Az Etkili ❌) |
|---|------|---------------|-------------------------------------------|
| 1 | **Clear & Concise Questions** | Soruları kısa ve net yaz. | ✅ “How do I make spaghetti carbonara?” <br> ❌ “I've been pondering over the possibility of engaging in a culinary activity involving pasta...” |
| 2 | **Provide Adequate Context** | Bağlam ver, arka planı açıkla. | ✅ “I’m analyzing social media with Python, data collection bitti. Next step?” <br> ❌ “What should I do next in my project?” |
| 3 | **Be Specific** | Genel değil, özel sorular sor. | ✅ “Explain Python list comprehensions.” <br> ❌ “Tell me about Python.” |
| 4 | **Closed-Ended Questions** | Net bilgi için kapalı uçlu sorular sor. | ✅ “How many planets are in the solar system?” <br> ❌ “What can you tell me about the solar system?” |
| 5 | **Open-Ended Questions** | Fikir ve keşif için açık uçlu sorular sor. | ✅ “Brainstorm sci-fi story ideas set in the future.” <br> ❌ “Do you have any story ideas?” |
| 6 | **Iterative Refinement** | Adım adım promptu geliştir. | ✅ “How can I improve my site?” → “Suggest color schemes for a tech blog.” |
| 7 | **Avoid Bias** | Tarafsız sor, yönlendirme yapma. | ✅ “What are pros & cons of Python?” <br> ❌ “Why is Python the best language?” |
| 8 | **Know AI’s Limits** | Yapılabilir şeyler iste. | ✅ “Summarize climate change in 500 words.” <br> ❌ “Write a 10,000-word essay.” |
| 9 | **Clarify Ambiguities** | Belirsiz cevapları netleştir. | ✅ “Data is in CSV, what next?” <br> ❌ “The next step depends on your data format.” (AI cevabı) |
| 10 | **Balance Detail & Brevity** | Ne çok uzun ne çok kısa prompt yaz. | ✅ “Recommended diet for active 3-year-old outdoor cat?” <br> ❌ “My cat Whiskers is 3 years old, loves outside... what food?” |

## 📌 Prompt Priming – Quick Reference

Aşağıdaki tablo, prompt priming tekniğinin yapay zekâ yanıtlarını nasıl etkilediğini örneklerle göstermektedir.

| # | Tür | Açıklama | Örnek Prompt |
|---|-----|----------|--------------|
| 1 | **Without Creative Writing Priming** | Bağlam verilmez, AI genel ve klişe içerik üretir. | ❌ “Write a story about dragons and elves.” |
| 2 | **Creative Writing Priming** | Ayrıntılı sahne, karakter ve olay örgüsü verilir; AI daha yaratıcı ve özgün cevap üretir. | ✅ “Imagine a mystical world where dragons and elves coexist… Write a story about a young elf named Elara.” |
| 3 | **Without Technical Explanation Priming** | Genel ve teknik açıklama gelir; hedef kitleye uygun olmayabilir. | ❌ “Explain machine learning.” |
| 4 | **Technical Explanation Priming** | Hedef kitle, tarz ve dil belirtilir; AI daha anlaşılır ve uyumlu cevap üretir. | ✅ “Explain machine learning as if teaching high school students, using simple analogies.” |

## 📌 General Prompt Frameworks – Quick Reference

Aşağıdaki tablo, etkili prompt oluşturmak için kullanılabilecek genel çerçeveleri (frameworks) örneklerle özetlemektedir.

| # | Framework | Açıklama | Örnek Prompt |
|---|-----------|----------|--------------|
| 1 | **RGC (Role, Goals, Context)** | AI’nın rolünü, hedefi ve bağlamı netleştirir. | ✅ “You are a travel advisor. I'm planning a trip to Japan for two weeks in April. My goals are to experience traditional Japanese culture and visit cherry blossom sites. What itinerary would you suggest?” |
| 2 | **Constraint-Led Framework** | Cevap için belirli kısıtlamalar koyarak yaratıcılığı yönlendirir. | ✅ “Write a poem about the ocean, but use only four-line stanzas and avoid the words 'sea', 'water', or 'blue'.” |
| 3 | **Open-Ended Exploration** | Geniş, yaratıcı ve farklı olasılıkları araştırmayı teşvik eder. | ✅ “What might be some unexpected consequences of colonizing Mars?” |
| 4 | **Skill Demonstration** | AI’dan belirli bir becerisini veya uzmanlığını sergilemesini ister. | ✅ “As a chess instructor, analyze the 1972 game between Bobby Fischer and Boris Spassky, focusing on key moves and strategies.” |
| 5 | **Hypothetical Scenario** | Varsayımsal senaryolar üzerinden olası sonuçları keşfeder. | ✅ “Imagine if the internet was shut down worldwide for a month. How might this affect global communication and business?” |

## 📌 Focused Prompt Frameworks – Quick Reference

Aşağıdaki tablo, farklı kullanım amaçlarına göre odaklı prompt framework’lerini örnekleriyle özetlemektedir.

| # | Framework | Amaç | Örnek Prompt |
|---|-----------|------|--------------|
| 1 | **Information Retrieval** | Belirli bilgi/faktörleri öğrenmek | ✅ “What are the key differences between Python and JavaScript in terms of syntax and use-cases?” |
| 2 | **Creative Generation** | Orijinal, yaratıcı içerik üretmek | ✅ “Create a short story set in a futuristic city where technology controls nature, focusing on a protagonist who rebels against this system.” |
| 3 | **Problem-Solving** | Belirli bir soruna çözüm/strateji bulmak | ✅ “I'm struggling to increase engagement on my educational YouTube channel. What are some effective strategies to boost viewer interaction and retention?” |
| 4 | **Learning & Explanation** | Kavramları anlaşılır şekilde açıklamak | ✅ “Explain the concept of gravitational pull to a 10-year-old without using complex physics terms.” |
| 5 | **Opinion & Analysis** | Görüş, değerlendirme veya analiz almak | ✅ “Analyze the impact of social media on modern communication, focusing on both its benefits and drawbacks.” |
| 6 | **Instructional / How-To** | Adım adım rehber veya talimat vermek | ✅ “Describe the steps involved in baking a chocolate cake for someone who has never baked before.” |
| 7 | **Comparative Analysis** | Kavramları/teorileri karşılaştırmak | ✅ “Compare the economic policies of Keynesianism and Monetarism, highlighting their main principles and impacts on modern economies.” |
| 8 | **Scenario Simulation** | Varsayımsal senaryoları keşfetmek | ✅ “Imagine a scenario where renewable energy has completely replaced fossil fuels by 2050. How would this affect global economies and the environment?” |
| 9 | **Personal Advice** | Kişisel duruma özel öneriler almak | ✅ “I'm a college student majoring in computer science and feeling overwhelmed. How can I effectively manage my time and reduce stress?” |
| 10 | **Interactive Storytelling** | Kullanıcı etkileşimine dayalı hikâyeler oluşturmak | ✅ “Start a mystery story set in an abandoned mansion. I'll tell you what choices the main character makes at key points.” |


## 📌 Prompt Revisions – Quick Reference  

Aşağıdaki tablo, farklı revizyon türlerinde AI’dan neler istenebileceğini örneklerle özetlemektedir.  

| #  | Framework | Amaç | Örnek Prompt | AI’dan Ne İsteniyor? |
|----|-----------|------|--------------|----------------------|
| 1  | **Highlight Keywords** | Anahtar terimleri kalın yazarak vurgulamak | ✅ “Please bold the key terms that are most critical in this text…” | Kritik kelimeleri **bold** yapması |
| 2  | **Organize by Criteria** | İçeriği ölçütlere göre düzenlemek | ✅ “Arrange the content chronologically and categorize by date, location, and cost…” | Tarih, yer, maliyet gibi kategorilere ayırması |
| 3  | **Generate Unique Ideas** | Sıradışı, yaratıcı öneriler üretmek | ✅ “Can you provide some creative and less common suggestions for…” | Alışılmışın dışında fikirler sunması |
| 4  | **Add Emojis** | Metni emojilerle renklendirmek | ✅ “Add suitable emojis to enhance the expressiveness of this text…” | İçeriğe uygun emoji eklemesi |
| 5  | **Simplify for Young Audience** | Çocuklara uygun basit açıklamalar yapmak | ✅ “Could you explain this in a way that a 5-year-old would easily understand…” | Konuyu çocuk seviyesinde basitleştirmesi |
| 6  | **Format as Table** | Bilgiyi tabloya dönüştürmek | ✅ “Please present this data in a table, sorting it into relevant categories…” | Veriyi tablo halinde düzenlemesi |
| 7  | **Expert Viewpoint** | Uzman bakış açısıyla yazmak | ✅ “Rewrite this from the perspective of an expert in the field…” | Profesyonel ve teknik bir üslupla yeniden yazması |
| 8  | **Adjust Tone** | Üslubu değiştirmek (resmi/samimi) | ✅ “Please modify this to sound more formal/informal…” | Dil tonunu hedef kitleye uygun ayarlaması |
| 9  | **Fix Grammar & Replace Terms** | Hataları düzeltmek, kelime değiştirmek | ✅ “Correct any grammar mistakes and substitute the following terms with…” | Dilbilgisini düzeltmesi + verilen kelimeleri değiştirmesi |
| 10 | **Add Humor/Personality** | Metni eğlenceli hale getirmek | ✅ “Can you rewrite this to make it more engaging and humorous…” | Daha esprili, eğlenceli bir dille yazması |
| 11 | **Specific Perspective/Voice** | Belirli rol/karakter sesiyle yazmak | ✅ “Compose this from the viewpoint of [specified role/character]…” | Belirlenen kişi/rol bakış açısıyla yazması |
| 12 | **Condense to Tweet** | İçeriği tweet’e sığdırmak | ✅ “Summarize this information to fit into a tweet (280 characters)…” | İçeriği 280 karaktere özetlemesi |
| 13 | **Three-Part Summary** | Üç bölümlük özet yapmak | ✅ “Divide this into a three-part summary…” | İçeriği giriş, gelişme, sonuç gibi 3 parçaya bölmesi |
| 14 | **Comparative Analysis** | Karşılaştırma yapmak | ✅ “Compare and contrast the key elements…” | Benzerlik ve farklılıkları belirtmesi |
| 15 | **10 Key Takeaways** | En önemli 10 noktayı çıkarmak | ✅ “What are the 10 most important points…” | 10 maddelik özet liste oluşturması |
| 16 | **Expert Review** | Profesyonel geliştirme önerileri vermek | ✅ “From a professional standpoint, how would you suggest enhancing this…” | İçeriği değerlendirip iyileştirme tavsiyeleri sunması |
| 17 | **Bullet Points** | Madde işaretleriyle düzenlemek | ✅ “Please format this information into a clear, bullet-pointed list…” | İçeriği maddeler halinde listelemesi |
| 18 | **Translate** | Başka dile çevirmek | ✅ “Could you translate this text into [specified language]…” | Metni hedef dile çevirip anlamı koruması |
| 19 | **Visual/Infographic** | Görselleştirmek | ✅ “Turn this data into a visual infographic…” | İçeriği infografik/şema taslağına dönüştürmesi |
| 20 | **Executive Summary** | Yönetici özeti hazırlamak | ✅ “Compose a concise executive summary…” | Uzun içeriği kısa bir özet halinde sunması |
| 21 | **FAQs** | SSS listesi oluşturmak | ✅ “Can you create a list of frequently asked questions…” | İçerikten olası sorular üretip yanıtlaması |
| 22 | **Persuasive Argument** | İkna edici argüman yazmak | ✅ “Formulate a compelling argument either in support of or against…” | Belirtilen görüşü destekleyen/karşıt argüman geliştirmesi |
