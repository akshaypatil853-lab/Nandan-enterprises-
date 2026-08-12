<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NANDAN ENTERPRISES | महाराष्ट्रातील १ ले हायटेक डिजिटल पोर्टल</title>
    <!-- Modern Fonts & FontAwesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@800;900&family=Poppins:wght@400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #D32F2F;
            --primary-dark: #B71C1C;
            --secondary: #7B1FA2;
            --accent: #FFC107;
            --dark: #0F172A;
            --card-bg: #FFFFFF;
            --shadow: 0 20px 25px -5px rgba(0,0,0,0.1), 0 8px 10px -6px rgba(0,0,0,0.1);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Poppins', sans-serif; }
        body { background-color: #F8FAFC; color: var(--dark); line-height: 1.6; }

        /* 🔥 UNIQUE HEADER */
        header { 
            background: linear-gradient(135deg, #FFFDE7 0%, #FFF9C4 100%); 
            padding: 25px 15px; 
            text-align: center; 
            border-bottom: 5px solid var(--primary);
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
            position: relative;
        }
        .brand-box { display: flex; align-items: center; justify-content: center; gap: 12px; }
        .peacock-icon { font-size: 42px; filter: drop-shadow(0 4px 6px rgba(0,0,0,0.1)); }
        .brand-title { font-family: 'Montserrat', sans-serif; font-size: 40px; font-weight: 900; color: var(--primary); letter-spacing: 2px; }
        .sub-title { font-family: 'Montserrat', sans-serif; font-size: 18px; font-weight: 800; color: var(--secondary); letter-spacing: 5px; }
        .owner-tag { font-size: 13px; font-weight: 800; color: #0D47A1; background: #E3F2FD; display: inline-block; padding: 5px 20px; border-radius: 25px; margin-top: 10px; border: 1.5px dashed #0D47A1; }

        /* 🚀 REVOLUTIONARY HERO SECTION */
        .hero {
            background: linear-gradient(135deg, #1E1B4B 0%, #4C1D95 50%, #831843 100%);
            color: white;
            padding: 50px 20px 70px;
            text-align: center;
            border-radius: 0 0 35px 35px;
            box-shadow: var(--shadow);
        }
        .hero-badge { background: rgba(255, 255, 255, 0.15); backdrop-filter: blur(10px); padding: 6px 18px; border-radius: 20px; font-size: 12px; font-weight: 700; color: var(--accent); display: inline-block; margin-bottom: 15px; border: 1px solid rgba(255,255,255,0.2); }
        .hero h2 { font-size: 30px; font-weight: 900; line-height: 1.3; margin-bottom: 12px; }
        .hero p { font-size: 15px; opacity: 0.9; max-width: 650px; margin: 0 auto 25px; }

        /* Floating Stats Bar */
        .stats-bar {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
            gap: 15px;
            background: white;
            padding: 22px;
            border-radius: 20px;
            max-width: 1000px;
            margin: -45px auto 40px;
            box-shadow: var(--shadow);
            text-align: center;
            position: relative;
            z-index: 10;
            border: 1px solid #E2E8F0;
        }
        .stat-item h4 { color: var(--primary); font-size: 22px; font-weight: 900; }
        .stat-item p { font-size: 12px; color: #64748B; font-weight: 700; }

        .container { max-width: 1050px; margin: 0 auto; padding: 0 15px; }

        /* 👑 VIP FEATURED CARDS */
        .vip-card {
            background: white;
            border-radius: 24px;
            border: 2.5px solid var(--primary);
            padding: 28px;
            margin-bottom: 35px;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }
        .vip-badge { position: absolute; top: 18px; right: -32px; background: var(--accent); color: var(--dark); padding: 6px 40px; transform: rotate(45deg); font-size: 11px; font-weight: 900; letter-spacing: 1px; }

        /* GRID LAYOUT FOR SERVICES */
        .section-header { font-size: 22px; font-weight: 800; color: var(--dark); margin-bottom: 22px; display: flex; align-items: center; gap: 10px; }
        .section-header::before { content: ''; width: 7px; height: 26px; background: var(--primary); border-radius: 4px; }

        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(290px, 1fr)); gap: 22px; margin-bottom: 50px; }

        .card {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 24px;
            border: 1px solid #E2E8F0;
            box-shadow: 0 4px 6px -1px rgba(0,0,0,0.05);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .card:hover { transform: translateY(-8px); box-shadow: var(--shadow); border-color: var(--primary); }

        .card-icon { width: 52px; height: 52px; border-radius: 14px; background: #FFEBEE; color: var(--primary); display: flex; align-items: center; justify-content: center; font-size: 22px; margin-bottom: 15px; }
        .card-title { font-size: 18px; font-weight: 800; color: var(--dark); margin-bottom: 8px; }
        .card-desc { font-size: 13px; color: #64748B; margin-bottom: 18px; line-height: 1.6; }

        .btn-card {
            display: block;
            width: 100%;
            padding: 12px;
            border-radius: 12px;
            text-align: center;
            text-decoration: none;
            font-weight: 700;
            font-size: 13px;
            transition: 0.2s;
            border: none;
            cursor: pointer;
        }

        footer { background: var(--dark); color: white; text-align: center; padding: 30px 15px; margin-top: 50px; font-size: 13px; }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <div class="brand-box">
            <span class="peacock-icon">🪶</span>
            <span class="brand-title">NANDAN</span>
        </div>
        <div class="sub-title">ENTERPRISES</div>
        <div class="owner-tag">🏢 नंदकुमार आप्पासो पाटील { एंटरप्राइजेस }</div>
    </header>

    <!-- HERO SECTION -->
    <div class="hero">
        <div class="hero-badge">⚡ महाराष्ट्रातील पहिले AI-रेडी सेवा पोर्टल</div>
        <h2>एकाच प्लॅटफॉर्मवर सर्व सोयी,<br>मध्यस्थांशिवाय (0% Brokerage)!</h2>
        <p>विवाह जुळवणी, कायदेशीर व्हिडिओ सल्ला, घरे-गाड्या खरेदी-विक्री आणि लोकल बिझनेस प्रमोशन.</p>
    </div>

    <!-- STATS BAR -->
    <div class="stats-bar">
        <div class="stat-item">
            <h4>१००%</h4>
            <p>व्हेरीफाईड डेटा</p>
        </div>
        <div class="stat-item">
            <h4>०%</h4>
            <p>दलाली / ब्रोकरेज</p>
        </div>
        <div class="stat-item">
            <h4>इन्स्टंट</h4>
            <p>व्हिडिओ कॉल सोय</p>
        </div>
    </div>

    <div class="container">

        <!-- VIP 1: विवाह जुळवणी -->
        <div class="vip-card">
            <div class="vip-badge">PREMIUM</div>
            <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 10px; margin-bottom: 15px;">
                <div style="display: flex; gap: 15px; align-items: center;">
                    <div class="card-icon" style="background: #FFE0B2; color: #E65100; margin: 0;">
                        <i class="fa-solid fa-heart"></i>
                    </div>
                    <div>
                        <h3 style="font-size: 22px; font-weight: 800; color: #1E293B;">💐 नंदन हायटेक विवाह जुळवणी</h3>
                        <p style="font-size: 13px; color: #E65100; font-weight: 700;">मध्यस्थांचे (Brokers) हजारो रुपये वाचवा!</p>
                    </div>
                </div>
                <span style="background: var(--primary); color: white; padding: 6px 16px; border-radius: 20px; font-weight: bold; font-size: 14px;">वार्षिक फी: ₹५,०००</span>
            </div>
            
            <p style="font-size: 14px; color: #475569; margin-bottom: 20px;">
                ✨ **खास वैशिष्ट्ये:** सर्व जातींच्या वधू-वरांची सोय, पालकांशी थेट फोन जोडणी आणि घरबसल्या **सुरक्षित HD व्हिडिओ कॉलची** अद्वितीय सोय!
            </p>
            <a href="#" class="btn-card" style="background: var(--primary); color: white;">📝 ऑनलाईन बायोडाटा नोंदणी करा ➔</a>
        </div>

        <div class="section-header">मुख्य सेवा विभाग</div>

        <div class="services-grid">
            
            <!-- VIP 2: वकील कक्ष -->
            <div class="card" style="border: 2px solid #0D47A1;">
                <div>
                    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px;">
                        <div class="card-icon" style="background: #E3F2FD; color: #0D47A1; margin: 0;"><i class="fa-solid fa-scale-balanced"></i></div>
                        <span style="background: #0D47A1; color: white; padding: 4px 10px; border-radius: 12px; font-size: 11px; font-weight: bold;">२ महिने FREE Trial</span>
                    </div>
                    <div class="card-title">⚖️ नंदन वकील कक्ष</div>
                    <div class="card-desc">
                        <b>संस्थापक:</b> ॲड. श्रीराज नंदकुमार पाटील.<br>
                        • वकिलांसाठी २ महिने मोफत नोंदणी (नंतर ₹१०,०००/वर्ष).<br>
                        • ग्राहकांसाठी कायदेशीर व्हिडिओ सल्ला: <b>₹१० / २ मिनिटे</b>.
                    </div>
                </div>
                <a href="#" class="btn-card" style="background: #0D47A1; color: white;">📹 व्हिडिओ सल्ला / वकील नोंदणी ➔</a>
            </div>

            <!-- VIP 3: जाहिरात हब -->
            <div class="card" style="border: 2px solid #E65100;">
                <div>
                    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px;">
                        <div class="card-icon" style="background: #FFF3E0; color: #E65100; margin: 0;"><i class="fa-solid fa-bullhorn"></i></div>
                        <span style="background: #E65100; color: white; padding: 4px 10px; border-radius: 12px; font-size: 11px; font-weight: bold;">डिजिटल प्रमोशन</span>
                    </div>
                    <div class="card-title">📢 शाळा, कॉलेज व व्यवसाय जाहिरात</div>
                    <div class="card-desc">
                        • 🎓 <b>कॉलेज जाहिरात:</b> ₹२,००० / महिना<br>
                        • 🏫 <b>शाळा जाहिरात:</b> ₹१,००० / महिना<br>
                        • 🏪 <b>इतर व्यवसाय:</b> ₹७०० / महिना
                    </div>
                </div>
                <a href="#" class="btn-card" style="background: #E65100; color: white;">📞 जाहिरात बुक करा ➔</a>
            </div>

            <!-- VIP 4: रिअल इस्टेट -->
            <div class="card" style="border: 2px solid #2E7D32;">
                <div>
                    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px;">
                        <div class="card-icon" style="background: #E8F5E9; color: #2E7D32; margin: 0;"><i class="fa-solid fa-house-chitin"></i></div>
                        <span style="background: #2E7D32; color: white; padding: 4px 10px; border-radius: 12px; font-size: 11px; font-weight: bold;">जाहिरात फी: ₹२,०००</span>
                    </div>
                    <div class="card-title">🏡 नंदन रिअल इस्टेट हब</div>
                    <div class="card-desc">शेती, घरे व प्लॉट्स थेट मालकाकडून खरेदी-विक्री करा. ०% दलाली. जाहिरात फी फक्त ₹२,०००.</div>
                </div>
                <a href="#" class="btn-card" style="background: #2E7D32; color: white;">🏡 जाहिरात टाका ➔</a>
            </div>

            <!-- VIP 5: जुन्या गाड्या -->
            <div class="card" style="border: 2px solid #0288D1;">
                <div>
                    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px;">
                        <div class="card-icon" style="background: #E1F5FE; color: #0288D1; margin: 0;"><i class="fa-solid fa-car"></i></div>
                        <span style="background: #0288D1; color: white; padding: 4px 10px; border-radius: 12px; font-size: 11px; font-weight: bold;">जाहिरात फी: ₹५००</span>
                    </div>
                    <div class="card-title">🚗 जुन्या गाड्या हब</div>
                    <div class="card-desc">टू-व्हिलर व फोर-व्हिलर गाड्यांची थेट मालकाशी बोलून खरेदी-विक्री करा. जाहिरात फी ₹५००.</div>
                </div>
                <a href="#" class="btn-card" style="background: #0288D1; color: white;">🚗 जाहिरात टाका ➔</a>
            </div>

            <!-- इतर नेहमीच्या सेवा -->
            <div class="card">
                <div>
                    <div class="card-icon"><i class="fa-solid fa-building-columns"></i></div>
                    <div class="card-title">🏦 कर्ज सहाय्यता केंद्र</div>
                    <div class="card-desc">होम लोन, वैयक्तिक कर्ज व बिझनेस लोनसाठी ऑनलाईन मदत.</div>
                </div>
                <a href="#" class="btn-card" style="background: #F8FAFC; color: var(--dark); border: 1px solid #CBD5E1;">अर्जाची पात्रता तपासा ➔</a>
            </div>

            <div class="card">
                <div>
                    <div class="card-icon"><i class="fa-solid fa-credit-card"></i></div>
                    <div class="card-title">💳 क्रेडिट कार्ड सेवा</div>
                    <div class="card-desc">इन्स्टंट कॅश प्रोसेसिंग आणि सिबिल (CIBIL) चेक सोय.</div>
                </div>
                <a href="#" class="btn-card" style="background: #F8FAFC; color: var(--dark); border: 1px solid #CBD5E1;">कार्ड सेवा पहा ➔</a>
            </div>

            <div class="card">
                <div>
                    <div class="card-icon"><i class="fa-solid fa-seedling"></i></div>
                    <div class="card-title">🌾 सेंद्रिय शेती हब</div>
                    <div class="card-desc">वेस्टिज, रियांश व मल्टिप्लायर खतांसाठी तज्ज्ञ सल्ला.</div>
                </div>
                <a href="#" class="btn-card" style="background: #F8FAFC; color: var(--dark); border: 1px solid #CBD5E1;">सेंद्रिय उत्पादने ➔</a>
            </div>

            <div class="card">
                <div>
                    <div class="card-icon"><i class="fa-solid fa-user-graduate"></i></div>
                    <div class="card-title">🎓 शिक्षण & DKTE प्रवेश</div>
                    <div class="card-desc"><b>मार्गदर्शक:</b> मनोज श्रेणिक उपाध्ये. इंजिनिअरिंग प्रवेश मदत.</div>
                </div>
                <a href="#" class="btn-card" style="background: #F8FAFC; color: var(--dark); border: 1px solid #CBD5E1;">प्रवेश मदत ➔</a>
            </div>

        </div>

    </div>

    <!-- FOOTER -->
    <footer>
        <p>© 2026 NANDAN ENTERPRISES | महाराष्ट्रातील पहिले ऑल-इन-वन सेवा पोर्टल</p>
        <p style="font-size: 11px; opacity: 0.7; margin-top: 5px;">नंदकुमार आप्पासो पाटील { एंटरप्राइजेस }</p>
    </footer>

</body>
</html>
