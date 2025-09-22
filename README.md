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
