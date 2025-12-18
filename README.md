

<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <title>4A 打造您的領導力｜導讀</title>

    <style>
        :root {
            --primary: #4338ca;
            --secondary: #0ea5a4;
            --bg: #f8fafc;
            --card: #ffffff;
            --text: #1f2937;
            --muted: #64748b;
        }

        body {
            margin: 0;
            font-family: "Segoe UI", Arial, sans-serif;
            background: var(--bg);
            color: var(--text);
            line-height: 1.8;
        }

        header {
            background: linear-gradient(135deg, var(--primary), #6366f1);
            color: white;
            padding: 70px 20px;
            text-align: center;
        }

        header h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        main {
            max-width: 1000px;
            margin: 50px auto;
            padding: 0 20px;
        }

        .chapter {
            background: var(--card);
            border-radius: 16px;
            padding: 28px;
            margin-bottom: 24px;
            box-shadow: 0 12px 30px rgba(0,0,0,0.08);
        }

        .chapter-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            cursor: pointer;
        }

        .chapter-header h2 {
            color: var(--primary);
            margin: 0;
        }

        .toggle-btn {
            background: var(--secondary);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 30px;
            font-size: 14px;
            cursor: pointer;
            transition: 0.3s;
        }

        .toggle-btn:hover {
            background: #0d9488;
        }

        .content {
            display: none;
            margin-top: 20px;
        }

        ul {
            padding-left: 20px;
        }

        li {
            margin-bottom: 10px;
        }

        .highlight {
            background: #eef2ff;
            border-left: 6px solid var(--primary);
            padding: 16px 20px;
            margin: 20px 0;
            border-radius: 10px;
            font-weight: bold;
        }

        .quote {
            background: #f1f5f9;
            padding: 20px;
            border-radius: 12px;
            font-style: italic;
            margin: 20px 0;
        }

        footer {
            text-align: center;
            color: var(--muted);
            padding: 40px 10px;
            font-size: 14px;
        }
    </style>
</head>

<body>

<header>
    <h1>4A 打造您的領導力</h1>
    <p>導讀 1/2｜章節點擊展開式學習</p>
</header>

<main>

    <!-- Chapter 1 -->
    <div class="chapter">
        <div class="chapter-header">
            <h2>領導 vs 管理</h2>
            <button class="toggle-btn" onclick="toggleContent(this)">查看內容</button>
        </div>
        <div class="content">
            <p><strong>領導力</strong>：透過討論與想法交流來引導團隊。</p>
            <p><strong>管理</strong>：使用一組規定的行為來指導行動。</p>

            <div class="highlight">
                領導關注的是「人與方向」，管理關注的是「規則與流程」。
            </div>
        </div>
    </div>

    <!-- Chapter 2 -->
    <div class="chapter">
        <div class="chapter-header">
            <h2>僕人式領導（1.2.3）</h2>
            <button class="toggle-btn" onclick="toggleContent(this)">查看內容</button>
        </div>
        <div class="content">
            <p>
                僕人式領導的核心不是「我怎麼管人」，而是
                <strong>「我怎麼讓團隊更容易成功」</strong>。
            </p>

            <ul>
                <li>促進而非管理 → 讓事情更順</li>
                <li>提供輔導與培訓 → 提前協助成長</li>
                <li>消除工作障礙 → 領導者是擋風的人</li>
                <li>專注於成就 → 成功歸功於團隊</li>
                <li>鼓勵每個人成為僕人式領導</li>
            </ul>

            <div class="quote">
                僕人式領導不是把權力放下，而是把力量放到團隊身上。
            </div>
        </div>
    </div>

    <!-- Chapter 3 -->
    <div class="chapter">
        <div class="chapter-header">
            <h2>領導風格五種類型（1.2.4）</h2>
            <button class="toggle-btn" onclick="toggleContent(this)">查看內容</button>
        </div>
        <div class="content">
            <ul>
                <li>直接型：我說了算，你照做</li>
                <li>諮詢型：一起討論，再做決定</li>
                <li>僕人式：方向給你，怎麼做你決定</li>
                <li>共識 / 協作型：一起決定，一起負責</li>
                <li>情境型：沒有最好，只有最適合</li>
            </ul>
        </div>
    </div>

    <!-- Chapter 4 -->
    <div class="chapter">
        <div class="chapter-header">
            <h2>虛擬團隊的參與與支援（1.11）</h2>
            <button class="toggle-btn" onclick="toggleContent(this)">查看內容</button>
        </div>
        <div class="content">
            <p>
                虛擬團隊最大的挑戰不是技術，而是<strong>「人之間的連結感」</strong>。
            </p>

            <ul>
                <li>管理孤立感 → 主動關心與互動</li>
                <li>聚焦團隊成果 → 我們一起完成了什麼</li>
                <li>建立共同承諾 → 在同一條船上</li>
            </ul>
        </div>
    </div>

</main>

<footer>
    學習導讀整理｜製作：芳芳
</footer>

<script>
    function toggleContent(button) {
        const content = button.parentElement.nextElementSibling;
        const isOpen = content.style.display === "block";

        content.style.display = isOpen ? "none" : "block";
        button.textContent = isOpen ? "查看內容" : "收合內容";
    }
</script>

</body>
</html>
