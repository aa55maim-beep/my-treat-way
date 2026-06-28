# 取り扱い説明書

        body {
            font-family: "Helvetica Neue", Arial, "Hiragino Kaku Gothic ProN", "Hiragino Sans", Meiryo, sans-serif;
            background-color: #fdfafb;
            color: #4a4a4a;
            margin: 0;
            padding: 0;
            line-height: 1.8;
            overflow-x: hidden;
        }

        /* 項目が浮かぶエリア */
        .bubble-container {
            width: 100%;
            height: auto;
            margin: 0 auto;
            position: relative;
            background: radial-gradient(circle at 50% 50%, #ffffff, #fdfafb);
            padding: 40px 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }

        .title-main {
            text-align: center;
            font-size: clamp(20px, 5vw, 28px);
            color: #5a5a5a;
            letter-spacing: 2px;
            margin-bottom: 10px;
            font-weight: bold;
            width: 100%;
        }

        /* バブルグリッドコンテナ */
        .bubble-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
            gap: 15px;
            width: 100%;
            max-width: 500px;
            margin: 0 auto;
            padding: 0 10px;
        }

        /* 浮かぶ丸ボタンの共通スタイル */
        .bubble-item {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            font-size: clamp(12px, 3vw, 14px);
            font-weight: bold;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.04);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
            text-align: center;
            position: relative;
            min-height: 100px;
        }

        /* ホバー（タップ）したときの動き */
        .bubble-item:hover,
        .bubble-item:active {
            transform: scale(1.1);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
        }

        .bubble-item span {
            display: block;
            line-height: 1.2;
        }

        .bubble-item span:first-child {
            font-size: clamp(24px, 6vw, 32px);
            margin-bottom: 4px;
        }

        /* 各バブルの色（まじめトーンのパステルカラー） */
        .b-profile {
            background-color: #fff0f2;
            color: #e07a8c;
        }
        .b-partner {
            background-color: #f0f7ff;
            color: #6ba4e8;
        }
        .b-happy {
            background-color: #fff9e6;
            color: #e6a817;
        }
        .b-kaeru {
            background-color: #f3f0ff;
            color: #9a7bee;
        }
        .b-action {
            background-color: #f0fdf4;
            color: #52b774;
        }

        /* 説明文のコンテンツエリア */
        .content-container {
            max-width: 100%;
            margin: 0 auto;
            padding: 0 15px 40px 15px;
        }

        .section-card {
            background: #ffffff;
            border-radius: 12px;
            padding: 20px 16px;
            margin-bottom: 20px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.02);
            border: 1px solid #f5efef;
            scroll-margin-top: 20px;
        }

        .section-card h2 {
            font-size: clamp(16px, 4vw, 18px);
            margin: 0 0 15px 0;
            padding-bottom: 10px;
            border-bottom: 2px solid #fdf4f5;
        }

        /* 各セクションのテーマカラー設定 */
        .section-card.p-profile h2 { color: #e07a8c; border-bottom-color: #fff0f2; }
        .section-card.p-partner h2 { color: #6ba4e8; border-bottom-color: #f0f7ff; }
        .section-card.p-happy h2 { color: #e6a817; border-bottom-color: #fff9e6; }
        .section-card.p-kaeru h2 { color: #9a7bee; border-bottom-color: #f3f0ff; }
        .section-card.p-action h2 { color: #52b774; border-bottom-color: #f0fdf4; }

        ul {
            padding-left: 18px;
            margin: 10px 0 0 0;
        }

        li {
            margin-bottom: 10px;
            font-size: clamp(13px, 3.5vw, 14.5px);
            color: #555555;
            line-height: 1.6;
        }

        strong {
            font-weight: bold;
        }
        
        .p-profile strong { color: #d65a6f; }
        .p-partner strong { color: #4b86d1; }
        .p-happy strong { color: #c98f0c; }
        .p-kaeru strong { color: #7e5cc9; }
        .p-action strong { color: #3b9c5b; }

        .footer {
            text-align: center;
            font-size: clamp(10px, 2.5vw, 11px);
            color: #bbb;
            margin-top: 40px;
            padding-bottom: 20px;
        }

        /* タブレット以上の画面用 */
        @media (min-width: 768px) {
            .bubble-container {
                max-width: 800px;
                height: 480px;
                padding-top: 40px;
            }

            .bubble-grid {
                display: contents;
            }

            .bubble-item {
                position: absolute;
                width: 110px;
                height: 110px;
            }

            .b-profile {
                top: 110px;
                left: 12%;
            }
            .b-partner {
                top: 90px;
                left: 42%;
            }
            .b-happy {
                top: 130px;
                right: 12%;
            }
            .b-kaeru {
                top: 270px;
                left: 25%;
            }
            .b-action {
                top: 290px;
                right: 28%;
            }

            .content-container {
                max-width: 650px;
                padding: 0 20px 100px 20px;
            }

            .section-card {
                padding: 30px 25px;
                margin-bottom: 40px;
            }

            .section-card h2 {
                font-size: 18px;
            }

            li {
                font-size: 14.5px;
            }
        }
    </style>
</head>
<body>

    <div class="bubble-container">
        <div class="title-main">まいの取扱説明書</div>
        
        <div class="bubble-grid">
            <a href="#profile" class="bubble-item b-profile">
                <span>🌸</span>
                <span>基本情報</span>
            </a>
            <a href="#partner" class="bubble-item b-partner">
                <span>🍳</span>
                <span>得意なこと</span>
            </a>
            <a href="#happy" class="bubble-item b-happy">
                <span>🍈</span>
                <span>されると嬉しいこと</span>
            </a>
            <a href="#kaeru" class="bubble-item b-kaeru">
                <span>⚠️</span>
                <span>蛙化しちゃうポイント</span>
            </a>
            <a href="#action" class="bubble-item b-action">
                <span>📢</span>
                <span>けんかしたら</span>
            </a>
        </div>
    </div>

    <div class="content-container">

        <div id="profile" class="section-card p-profile">
            <h2>🌸 1. 基本情報</h2>
            <ul>
                <li><strong>性格</strong>：好きなものはとことん好き</li>
                <li><strong>自己肯定感</strong>：高くも低くもない</li>
                <li><strong>モットー</strong>：真面目にふざける</li>
            </ul>
        </div>

        <div id="partner" class="section-card p-partner">
            <h2>🍳 2. 得意なこと</h2>
            <ul>
                <li><strong>料理</strong>：健康にします</li>
                <li><strong>マッサージ</strong>：痛がってても手加減しません</li>
                <li><strong>悩みを聞く</strong>：いつでも聞きます</li>
            </ul>
        </div>

        <div id="happy" class="section-card p-happy">
            <h2>🍈 3. されるとうれしいこと</h2>
            <ul>
                <li><strong>誘ってもらうこと</strong>：電話とかデートとか、提案してもらえると喜びます</li>
                <li><strong>メロンを食べさせてもらう</strong>：いくらでも食べれます</li>
            </ul>
        </div>

        <div id="kaeru" class="section-card p-kaeru">
            <h2>⚠️ 4. 蛙化しちゃうポイント</h2>
            <ul>
                <li>過去に関係のあった女性に会われること</li>
                <li>自分の保身のために嘘をつかれること</li>
                <li>雑に扱われたとき</li>
            </ul>
        </div>

        <div id="action" class="section-card p-action">
            <h2>📢 5.けんかしたら</h2>
            <ul>
                <li><strong>怒ったときの反応</strong>：ぷんぷん文句を言いますが、嫌いになったからじゃなくて好きだからこその行動です</li>
                <li><strong>不機嫌時の対処</strong>：私のためにPDCA回してください</li>
            </ul>
        </div>
    </div>

</body>
</html>
