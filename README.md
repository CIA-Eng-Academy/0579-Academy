
<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>0579 Academy</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: #f9f9f9;
            color: #333;
            line-height: 1.6;
            text-align: center;
        }

        header {
            background: #004080;
            color: white;
            text-align: center;
            padding: 20px;
        }

        header h1 {
            margin: 0;
        }

        /* Ticker */
        .ticker {
            overflow: hidden;
            background: #eee;
            white-space: nowrap;
            box-sizing: border-box;
            border-top: 2px solid #004080;
            border-bottom: 2px solid #004080;
        }

        .ticker p {
            display: inline-block;
            padding-left: 100%;
            animation: ticker 20s linear infinite;
            margin: 0;
        }

        @keyframes ticker {
            0% {
                transform: translateX(0);
            }

            100% {
                transform: translateX(-100%);
            }
        }

        /* Accordion */
        .accordion {
            background: #004080;
            color: white;
            cursor: pointer;
            padding: 15px;
            width: 80%;
            border: none;
            text-align: center;
            outline: none;
            font-size: 18px;
            transition: background 0.3s ease;
            margin: 10px auto;
            display: block;
            border-radius: 5px;
        }

        .accordion:hover {
            background: #0066cc;
        }

        .panel {
            padding: 10px;
            display: none;
            background: #f1f1f1;
            overflow: hidden;
            width: 80%;
            margin: 0 auto;
            border-radius: 5px;
        }

        .panel p,
        .panel ul,
        .panel ol {
            padding: 10px 0;
            margin: 0 auto;
            text-align: center;
            list-style-position: inside;
        }

        section {
            padding: 20px;
        }

        footer {
            background: #222;
            color: white;
            text-align: center;
            padding: 15px;
            font-size: 14px;
        }
    </style>
</head>

<body>

    <header>
        <h1>0579 Academy</h1>
        <p>"0579 학원에 오신 것을 환영합니다."</p>
    </header>

    <!-- Ticker 1 -->
    <div class="ticker">
        <p>공지사항: 9월 신학기 등록이 시작되었습니다! | 상담시간: 오전 9시부터 오후 3시 010-4733-0579로 상담신청 문자 남겨주시면 잔화드리겠습니다.</p>
    </div>

    <section>
        <h2>About 0579</h2>
        <p><b>0579 — 0579 Academy </b> is an English learning platform designed for students who want to master English for daily life, academic study, and professional success...</p>
        <!-- Insert an image (uploaded on GitHub) -->
        <img src="https://raw.githubusercontent.com/username/repository-name/main/images/about-image.jpg" alt="CIA English Academy" style="width: 100%; max-width: 500px;">
    </section>

    <!-- Accordion Sections -->
    <button class="accordion">Our 1:1 Service Menu</button>
    <div class="panel">
        <ol>
            <li>레벨 테스트</li>
            <li>프리토킹</li>
            <li>발음교정</li>
            <li>문법강의</li>
            <li>영어일기쓰기 교정</li>
            <li>모의고사 쪽집게 풀이</li>
            <li>Toeic, Toefl, IELTS 시험 준비반</li>
            <li>듣기, 말하기, 독해, 작문</li>
            <li>영어논문 및 연설글 준비</li>
            <li>CIA 특별강의 A.I. Mobile 학습법</li>
        </ol>
    </div>

    <button class="accordion">0579 Academy 학생 규정 및 환불규정</button>
    <div class="panel">
        <ol>
            <li>강의 및 학습이 어려운 경우, 즉시 귀가조치</li>
            <li>단정한 복장 착용과 예의바른 언어사용</li>
            <li>단순 변심으로 인한 수업 중단 시 환불 규정 적용</li>
        </ol>
    </div>

    <button class="accordion">특별 서비스</button>
    <div class="panel">
        <ul>
            <li>24 hours English Radio</li>
            <li>24 hours chatting</li>
            <li>24 hours Online Daily Diary checker</li>
        </ul>
    </div>

    <button class="accordion">강의노트</button>
    <div class="panel">
        <ul>
            <li>UPS Phonics (발음)</li>
            <li>Grammar Comprehension</li>
            <li>Listening Comprehension</li>
            <li>Speaking Comprehension</li>
            <li>Reading Comprehension</li>
            <li>Vocabulary Studies</li>
            <li>Writing Comprehension</li>
            <li>Pops English</li>
            <li>Movie English</li>
        </ul>
    </div>

    <button class="accordion">영어교재 및 영어교구</button>
    <div class="panel">
        <ul>
            <li>판매중인 교재</li>
            <li>예약판매중인 교재</li>
        </ul>
    </div>

    <button class="accordion">강사구인</button>
    <div class="panel">
        <p>Find English/Korean Native Teachers</p>
    </div>

    <button class="accordion">유튜브 강의</button>
    <div class="panel">
        <p>YouTube Video materials</p>
        <!-- Embed a YouTube video (change the link to your actual video) -->
        <iframe width="560" height="315" src="https://www.youtube.com/embed/your-video-id" frameborder="0" allowfullscreen></iframe>
    </div>

    <!-- Ticker 2 -->
    <div class="ticker" style="background: #dff0ff; color: #004080;">
        <p>"The pen is mightier than the sword." ✦ "Practice makes perfect." ✦ "Don’t put all your eggs in one basket." ✦ "Actions speak louder than words." ✦ "A journey of a thousand miles begins with a single step."</p>
    </div>

    <footer>
        <p>강의료 납부계좌: 기업은행 01047330579 오준영</p>
        <p>사이트 콘텐츠 무단사용 금지 | Copy Right Rules and Regulations</p>
    </footer>

    <script>
        // Accordion Script
        const acc = document.querySelectorAll(".accordion");

        acc.forEach(btn => {
            btn.addEventListener("click", function () {
                this.classList.toggle("active");
                const panel = this.nextElementSibling;
                panel.style.display = (panel.style.display === "block") ? "none" : "block";
            });
        });
    </script>
</body>

</html>
