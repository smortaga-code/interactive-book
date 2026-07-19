<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>استراتيجية بطل العرض الصغير</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@400;700&family=Afacad+Flux:wght@400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        * { box-sizing: border-box; }
        body { background-color: #f8fafc; margin: 0; display: grid; gap: 40px; place-items: center; padding: 40px 0; }
        
        .slide-container {
            width: 1280px; height: 720px;
            background-color: #ffffff; border-radius: 40px;
            box-shadow: 0 30px 60px rgba(0,0,0,0.1);
            overflow: hidden; position: relative;
            display: flex; flex-direction: column; padding: 60px 80px;
            font-family: 'Afacad Flux', sans-serif;
            z-index: 1;
        }

        .decoration-blob { position: absolute; border-radius: 50%; filter: blur(70px); z-index: -1; opacity: 0.4; }
        .blob-orange { width: 600px; height: 600px; background: #ff8b3d; top: -200px; right: -150px; }
        .blob-green { width: 500px; height: 500px; background: #d1ff00; bottom: -150px; left: -100px; }
        .blob-purple { width: 400px; height: 400px; background: #bc84ee; top: 150px; left: 150px; }

        h1, h2 { font-family: 'Comfortaa', cursive; color: #1e293b; margin: 0; }
        .slide-title { 
            font-size: 60px; font-weight: 700; color: #1e293b; margin-bottom: 40px; 
            text-align: right; width: 100%; border-right: 15px solid #ff8b3d; padding-right: 20px;
        }

        p, li, td, th { font-size: 26px; line-height: 1.5; color: #475569; }
        .content-area { flex-grow: 1; display: flex; flex-direction: column; justify-content: center; width: 100%; }
        
        .title-layout { text-align: center; justify-content: center; height: 100%; }
        .title-layout h1 { font-size: 110px; margin-bottom: 20px; color: #bc84ee; text-shadow: 4px 4px 0px rgba(188, 132, 238, 0.1); }
        .title-layout .cartoon-hero { width: 550px; height: 350px; margin: 20px auto; border-radius: 40px; overflow: hidden; border: 12px solid #d1ff00; background: #fff; }
        .title-layout .cartoon-hero img { width: 100%; height: 100%; object-fit: contain; }

        .two-column { display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: center; }
        .image-wrapper { width: 100%; height: 450px; border-radius: 50px; overflow: hidden; background: #fdfdfd; border: 8px dashed #bc84ee; }
        .image-wrapper img { width: 100%; height: 100%; object-fit: contain; }

        .tiled-content { display: grid; grid-template-columns: repeat(3, 1fr); gap: 30px; }
        .tile { padding: 40px 30px; border-radius: 50px; text-align: center; border-bottom: 10px solid #d1ff00; background: #f8fafc; }
        .tile .icon { font-size: 60px; color: #ff8b3d; margin-bottom: 25px; }

        .highlight-number-layout { display: flex; align-items: center; gap: 60px; }
        .big-number { font-size: 220px; font-weight: 700; color: #bc84ee; line-height: 1; font-family: 'Comfortaa'; }

        table { width: 100%; border-collapse: separate; border-spacing: 0 15px; }
        th { background-color: #bc84ee; color: white; padding: 25px; border-radius: 20px 0 0 20px; font-size: 32px; }
        td { background-color: #ffffff; padding: 20px; border: 3px solid #f1f5f9; text-align: center; }
        tr td:first-child { border-radius: 0 20px 20px 0; font-weight: 700; color: #059669; }
        tr td:last-child { border-radius: 20px 0 0 20px; color: #dc2626; }

        .timeline { display: flex; justify-content: space-between; position: relative; padding: 50px 0; }
        .timeline-line { position: absolute; top: 125px; left: 0; right: 0; height: 10px; background: #e2e8f0; border-radius: 5px; }
        .timeline-step { z-index: 1; width: 30%; text-align: center; }
        .step-dot { width: 50px; height: 50px; background: #ff8b3d; border-radius: 50%; border: 8px solid #fff; margin: 0 auto 30px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); }

        .qa-layout { text-align: center; justify-content: center; }
        .qa-layout h2 { font-size: 110px; color: #ff8b3d; margin-bottom: 40px; }
    </style>
</head>
<body>

    <div class="slide-container" id="slide1">
        <div class="decoration-blob blob-orange"></div>
        <div class="decoration-blob blob-purple"></div>
        <div class="title-layout">
            <h1>أنا بطل العرض!</h1>
            <p style="font-size: 38px; font-weight: 600;">كيف أشارك أصدقائي ما تعلمته بكل حماس؟</p>
            <div class="cartoon-hero">
                <img src="http://googleusercontent.com/image_collection/image_retrieval/1608796334473033648" alt="رسم كرتوني لطفل يقدم عرضاً مدرسياً بكل ثقة">
            </div>
            <p style="color: #64748b;">استراتيجيات بسيطة وممتعة لأبطال المرحلة الأساسية</p>
        </div>
    </div>

    <div class="slide-container" id="slide2" style="background-color: #d1ff00; justify-content: center; text-align: center; padding: 0;">
        <h2 style="font-size: 100px;">ما هو العرض الشفهي؟</h2>
        <p style="font-size: 44px; max-width: 900px; margin: 40px auto; line-height: 1.6;">هو "رحلة ممتعة" نأخذ فيها أصدقاءنا لنريهم الكنوز والمعلومات التي اكتشفناها في دروسنا!</p>
    </div>

    <div class="slide-container" id="slide3">
        <h2 class="slide-title">لماذا التقديم ممتع؟</h2>
        <div class="content-area">
            <div class="tiled-content">
                <div class="tile" style="background: #e2c6ff; border-color: #bc84ee;">
                    <div class="icon"><i class="fa-solid fa-face-laugh-beam"></i></div>
                    <h3>أنا واثق</h3>
                    <p>أتعلم كيف أتحدث بجرأة وفخر أمام الجميع.</p>
                </div>
                <div class="tile" style="background: #ffd6a5; border-color: #ff8b3d;">
                    <div class="icon"><i class="fa-solid fa-people-carry-box"></i></div>
                    <h3>أنا أشارك</h3>
                    <p>أهدي أصدقائي معلومات مفيدة لنتعلم معاً.</p>
                </div>
                <div class="tile" style="background: #dcfd8b; border-color: #a3cf00;">
                    <div class="icon"><i class="fa-solid fa-rocket"></i></div>
                    <h3>أنا خبير</h3>
                    <p>عندما أشرح موضوعي، أثبت أنني فهمته بذكاء.</p>
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide4">
        <h2 class="slide-title">الاستعداد للمغامرة</h2>
        <div class="content-area">
            <div class="two-column">
                <div class="image-wrapper">
                    <img src="http://googleusercontent.com/image_collection/image_retrieval/15180280669970550691" alt="رسم كرتوني لطفل يجهز لوحة عرض ملونة">
                </div>
                <div>
                    <h3>قبل أن تبدأ، تذكر:</h3>
                    <ul style="list-style: none; padding: 0;">
                        <li style="margin-bottom: 25px;"><i class="fa-solid fa-wand-magic-sparkles" style="margin-left: 15px; color: #ff8b3d;"></i> اختر صوراً ورسومات ملونة تجذب الأنظار.</li>
                        <li style="margin-bottom: 25px;"><i class="fa-solid fa-comments" style="margin-left: 15px; color: #ff8b3d;"></i> تدرب على الكلام مع دميتك المفضلة أو أهلك.</li>
                        <li style="margin-bottom: 25px;"><i class="fa-solid fa-heart" style="margin-left: 15px; color: #ff8b3d;"></i> فكر في قصة مشوقة تحكيها لأصدقائك.</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide5">
        <h2 class="slide-title">سر البطل: الابتسامة</h2>
        <div class="content-area">
            <div class="highlight-number-layout">
                <div class="big-number">100%</div>
                <div>
                    <h3 style="font-size: 44px; color: #bc84ee;">ابتسامتك تجذب القلوب!</h3>
                    <p>عندما تبتسم وتنظر في عيون أصدقائك، سيشعرون بالسعادة والراحة للاستماع إليك. قف بكل ثقة كأنك بطل خارق يوزع المعرفة!</p>
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide6">
        <h2 class="slide-title">صوتك هو "قوتك"</h2>
        <div class="content-area">
            <div class="two-column">
                <div>
                    <div style="background: #f1f5f9; padding: 40px; border-radius: 40px; border-right: 15px solid #ff8b3d;">
                        <h3>كيف أتحدث؟</h3>
                        <p><strong>وضوح:</strong> انطق الكلمات ببطء ليفهمك الجميع.</p>
                        <p><strong>تنوع:</strong> اجعل صوتك متحماساً أحياناً وهادئاً أحياناً.</p>
                        <p><strong>قوة:</strong> تأكد أن الجميع في الفصل يسمع نبرتك الواثقة.</p>
                    </div>
                </div>
                <div class="image-wrapper" style="border-radius: 50%; width: 450px; height: 450px; margin: 0 auto; border-color: #ff8b3d;">
                    <img src="http://googleusercontent.com/image_collection/image_retrieval/17775041611002726246" alt="رسم كرتوني لطفل يتحدث بحيوية وتعبيرات وجه معبرة">
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide7">
        <h2 class="slide-title">أدواتي السحرية للشرح</h2>
        <div class="content-area">
            <div class="tiled-content">
                <div class="tile" style="background: #fdf4ff;">
                    <div class="icon"><i class="fa-solid fa-paintbrush"></i></div>
                    <h3>رسوماتي</h3>
                    <p>لوحات ملونة رسمتها تعبر عن فكرتي.</p>
                </div>
                <div class="tile" style="background: #f0fdf4;">
                    <div class="icon"><i class="fa-solid fa-tv"></i></div>
                    <h3>عروضي</h3>
                    <p>صور وفيديوهات قصيرة أعرضها على الشاشة.</p>
                </div>
                <div class="tile" style="background: #fffbeb;">
                    <div class="icon"><i class="fa-solid fa-shapes"></i></div>
                    <h3>أشيائي</h3>
                    <p>مجسمات حقيقية يلمسها أصدقائي ليفهموا.</p>
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide8">
        <h2 class="slide-title">خريطة العرض الناجح</h2>
        <div class="content-area">
            <div class="timeline">
                <div class="timeline-line"></div>
                <div class="timeline-step">
                    <div class="step-dot"></div>
                    <h3>مرحباً أصدقائي</h3>
                    <p>أحيي الجميع وأخبرهم عن موضوعي.</p>
                </div>
                <div class="timeline-step">
                    <div class="step-dot" style="background: #bc84ee;"></div>
                    <h3>قصة معرفتي</h3>
                    <p>أشرح ما فهمته بأمثلة وصور ممتعة.</p>
                </div>
                <div class="timeline-step">
                    <div class="step-dot" style="background: #d1ff00;"></div>
                    <h3>شكراً لكم</h3>
                    <p>ألخص فكرتي وأشكرهم على الاستماع.</p>
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide9">
        <h2 class="slide-title">صديقي يسأل وأنا أجيب</h2>
        <div class="content-area">
            <div class="two-column">
                <div class="image-wrapper" style="border-style: solid; border-color: #d1ff00;">
                    <img src="http://googleusercontent.com/image_collection/image_retrieval/11683915761521204400" alt="رسم كرتوني لمجموعة أطفال يستمعون بابتسامة وفضول">
                </div>
                <div>
                    <h3>بطل العرض الذكي:</h3>
                    <ul style="list-style: none; padding: 0;">
                        <li style="margin-bottom: 25px;"><i class="fa-solid fa-ear-listen" style="margin-left: 15px; color: #bc84ee;"></i> يستمع للسؤال بكل هدوء واهتمام.</li>
                        <li style="margin-bottom: 25px;"><i class="fa-solid fa-lightbulb" style="margin-left: 15px; color: #bc84ee;"></i> يقول: "هذا سؤال رائع جداً، شكراً لك!"</li>
                        <li style="margin-bottom: 25px;"><i class="fa-solid fa-magnifying-glass" style="margin-left: 15px; color: #bc84ee;"></i> يبحث عن الإجابة لاحقاً إذا لم يعرفها.</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <div class="slide-container" id="slide10">
        <h2 class="slide-title">قواعد الأبطال في الفصل</h2>
        <div class="content-area">
            <table>
                <thead>
                    <tr>
                        <th>افعل (نعم!) ✅</th>
                        <th>لا تفعل (تجنب) ❌</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>انظر في وجوه أصدقائك بابتسامة</td>
                        <td>تنظر للأرض أو للجدار فقط</td>
                    </tr>
                    <tr>
                        <td>تحدث بوضوح ليفهمك الجميع</td>
                        <td>تحدث بسرعة كأنك في سباق</td>
                    </tr>
                    <tr>
                        <td>استمتع بتقديم ما تعلمته</td>
                        <td>تخف يديك في جيوبك بخجل</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>

    <div class="slide-container" id="slide11" style="padding: 0; position: relative;">
        <img src="http://googleusercontent.com/image_collection/image_retrieval/17119620642194276789" alt="رسم كرتوني لطفل يحتفل بنجاحه مع نجوم ملونة" style="width: 100%; height: 100%; object-fit: cover; opacity: 0.8;">
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center; width: 80%;">
            <h2 style="font-size: 100px; color: #1e293b; background: rgba(255,255,255,0.8); padding: 40px; border-radius: 40px;">أنت نجم العرض القادم!</h2>
            <p style="font-size: 40px; color: #1e293b; font-weight: 600; margin-top: 20px;">انطلق وشاركنا إبداعك بكل فخر</p>
        </div>
    </div>

    <div class="slide-container qa-layout" id="slide12">
        <div class="decoration-blob blob-green"></div>
        <h2>هل لديكم أسئلة يا أبطال؟</h2>
        <p style="font-size: 36px; color: #64748b; margin-top: 30px;">شكراً لكم على استماعكم الرائع!</p>
        <div style="margin-top: 50px; font-size: 100px; color: #bc84ee;">
            <i class="fa-solid fa-face-laugh-wink"></i>
        </div>
    </div>

</body>
</html>
