# my-treat-way
取り扱い説明書
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>まいの取扱説明書</title>
    <style>
        body {
            font-family: "Helvetica Neue", Arial, "Hiragino Kaku Gothic ProN", "Hiragino Sans", Meiryo, sans-serif;
            background-color: #fdfafb; /* ほんのり桜がかった上品な白 */
            color: #4a4a4a;
            margin: 0;
            padding: 0;
            line-height: 1.8;
            overflow-x: hidden;
        }

        /* 項目が浮かぶエリア */
        .bubble-container {
            width: 100%;
            max-width: 800px;
            height: 480px;
            margin: 0 auto;
            position: relative;
            background: radial-gradient(circle at 50% 50%, #ffffff, #fdfafb);
            padding-top: 40px;
        }

        .title-main {
            text-align: center;
            font-size: 24px;
            color: #5a5a5a;
            letter-spacing: 2px;
            margin-bottom: 20px;
            font-weight: bold;
        }

        /* 浮かぶ丸ボタンの共通スタイル */
        .bubble-item {
            position: absolute;
            width: 110px;
            height: 110px;
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            font-size: 14px;
            font-weight: bold;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.04);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
            text-align: center;
        }

        /* ホバー（タップ）したときの動き */
        .bubble-item:hover {
            transform: scale(1.08);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
        }

        .bubble-item span {
            margin-top: 4px;
        }

        /* 各バブルの配置と色（まじめトーンのパステルカラー） */
        .b-profile {
            background-color: #fff0f2; /* 薄ピンク */
            color: #e07a8c;
            top: 110px;
            left: 12%;
        }
        .b-partner {
            background-color: #f0f7ff; /* 薄青 */
            color: #6ba4e8;
            top: 90px;
            left: 42%;
        }
        .b-happy {
            background-color: #fff9e6; /* 薄黄 */
            color: #e6a817;
            top: 130px;
            right: 12%;
        }
        .b-kaeru {
            background-color: #f3f0ff; /* 薄紫 */
            color: #9a7bee;
            top: 270px;
            left: 25%;
        }
        .b-action {
            background-color: #f0fdf4; /* 薄緑 */
            color: #52b774;
            top: 290px;
            right: 28%;
        }

        /* 説明文のコンテンツエリア */
        .content-container {
            max-width: 650px;
            margin: 0 auto 100px auto;
            padding: 0 20px;
        }

        .section-card {
            background: #ffffff;
            border-radius: 16px;
            padding: 30px 25px;
            margin-bottom: 40px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.02);
            border: 1px solid #f5efef;
            scroll-margin-top: 30px; /* スクロールした時に上に少し余白を作る設定 */
        }

        .section-card h2 {
            font-size: 18px;
            margin-top: 0;
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
            padding-left: 20px;
            margin: 15px 0 0 0;
        }

        li {
            margin-bottom: 12px;
            font-size: 14.5px;
            color: #555555;
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
            font-size: 11px;
            color: #bbb;
            margin-top: 60px;
        }
    </style>
</head>
<body>

    <div class="bubble-container">
        <div class="title-main">まいの取扱説明書</div>
        
        <a href="#profile" class="bubble-item b-profile">
            <span>🌸</span>
            <span>自己認識</span>
        </a>
        <a href="#partner" class="bubble-item b-partner">
            <span>🧍‍♂️</span>
            <span>理想の相手</span>
        </a>
        <a href="#happy" class="bubble-item b-happy">
            <span>🍈</span>
            <span>うれしいこと</span>
        </a>
        <a href="#kaeru" class="bubble-item b-kaeru">
            <span>⚠️</span>
            <span>蛙化トリガー</span>
        </a>
        <a href="#action" class="bubble-item b-action">
            <span>📢</span>
            <span>感情と対処</span>
        </a>
    </div>

    <div class="content-container">

        <div id="profile" class="section-card p-profile">
            <h2>🌸 1. 基本的な性質と自己認識</h2>
            <ul>
                <li><strong>性格</strong>：基本的には真面目ですが、寂しがり屋で少しメンヘラな一面を持ち合わせています。</li>
                <li><strong>自己肯定感</strong>：高くも低くもなく、標準的です。</li>
                <li><strong>強み</strong>：身内と認めた相手に対しては、非常に優しく接します。</li>
                <li><strong>弱み</strong>：生理の周期において、一時的にパートナー以外の男性全般に対してうっすらと嫌悪感を抱く傾向があります。この期間の体調と心情への理解が必要です。</li>
            </ul>
        </div>

        <div id="partner" class="section-card p-partner">
            <h2>🧍‍♂️ 2. 理想のパートナー像</h2>
            <ul>
                <li><strong>必須条件</strong>：優しいこと。また、自分自身に一貫性がないと感じているため、ブレない一貫性を持っている人に安心感を覚えます。</li>
                <li><strong>体型</strong>：体重<strong>78kg前後</strong>で、お姫様抱っこができる体格を好みます。</li>
            </ul>
        </div>

        <div id="happy" class="section-card p-happy">
            <h2>🍈 3. されるとうれしいこと</h2>
            <ul>
                <li><strong>お姫様抱っこ</strong>：日常的なスキンシップや、安心感を得たいときにされると非常に喜びます。</li>
                <li><strong>メロンを食べさせてもらう</strong>：ただ食べるだけでなく、「食べさせてもらう」という甘えられるシチュエーションに幸福感を覚えます。</li>
            </ul>
        </div>

        <div id="kaeru" class="section-card p-kaeru">
            <h2>⚠️ 4. 蛙化（気持ちが冷める）のトリガー</h2>
            <ul>
                <li>過去に関係のあった女性（元カノなど）と会うこと</li>
                <li>自分の保身のために嘘をつくこと</li>
                <li>雑に扱われるなど、大切にされている実感が持てないとき</li>
            </ul>
        </div>

        <div id="action" class="section-card p-action">
            <h2>📢 5. 感情表現と対処法</h2>
            <ul>
                <li><strong>怒ったときの反応</strong>：不満があると「ぷんぷん」と文句を言います。これは嫌いになったわけではなく、「好きだからこそ」出る真面目に向き合いたいサインです。</li>
                <li><strong>不機嫌時の対処</strong>：放置されると不安が強まります。話を優しく聴く、あるいは上記の「お姫様抱っこ」を実行して安心させてください。</li>
            </ul>
        </div>

        <div class="footer">
            <p>© 2026 まいの取扱説明書 All Rights Reserved.</p>
        </div>
    </div>

</body>
</html>
