
<!-- 首頁主視覺 -->
<div class="hero" id="home">
  <h1>198 屆 PMP 導讀</h1>
  <button onclick="startGuide()">開始導讀</button>
</div>

<!-- 導讀內容 -->
<main id="guide">

  <div class="card">
    <h2 onclick="toggleContent(this)">領導力 vs 管理</h2>
    <div class="content">
      <p><strong>領導力</strong>：透過討論與想法交流來引導團隊。</p>
      <p><strong>管理</strong>：使用一組規定的行為來指導行動。</p>
      <div class="highlight">領導關注「人與方向」，管理關注「規則與流程」。</div>
    </div>
  </div>

  <div class="card">
    <h2 onclick="toggleContent(this)">僕人式領導 (1.2.3)</h2>
    <div class="content">
      <p>核心不是「我怎麼管人」，而是<strong>「我怎麼讓團隊更容易成功」</strong>。</p>
      <ul>
        <li>促進而非管理 → 事情更順，不是管得更緊</li>
        <li>提供輔導與培訓 → 提前協助成長</li>
        <li>消除工作障礙 → 領導者是擋風的人，不是加壓的人</li>
        <li>專注於成就 → 成功歸功於團隊</li>
        <li>鼓勵每個人成為僕人式領導 → 行為而非職稱</li>
      </ul>
      <div class="highlight">僕人式領導不是把權力放下，而是把力量放到團隊身上。</div>
    </div>
  </div>

  <div class="card">
    <h2 onclick="toggleContent(this)">領導風格五種類型 (1.2.4)</h2>
    <div class="content">
      <ul>
        <li>直接型：我說了算，你照做</li>
        <li>諮詢型：一起討論，再做決定</li>
        <li>僕人式：方向給你，怎麼做你決定</li>
        <li>共識/協作型：一起決定，一起負責</li>
        <li>情境型：沒有最好，只有最適合</li>
      </ul>
      <div class="highlight">領導力需依對象、情境切換模式。</div>
    </div>
  </div>

  <div class="card">
    <h2 onclick="toggleContent(this)">虛擬團隊參與與支援 (1.11)</h2>
    <div class="content">
      <p>虛擬團隊挑戰：<strong>人之間的連結感</strong>。</p>
      <ul>
        <li>管理孤立感 → 主動關心與互動</li>
        <li>聚焦團隊成果 → 我們一起完成了什麼</li>
        <li>建立共同承諾 → 不在同地，但在同一條船上</li>
      </ul>
    </div>
  </div>

</main>

<footer>198 屆 PMP 導讀 - by 芳芳</footer>

<script>
  function startGuide() {
    document.getElementById('home').style.display='none';
    document.getElementById('guide').style.display='block';
    window.scrollTo({top:0, behavior:'smooth'});
  }

  function toggleContent(el) {
    const content = el.nextElementSibling;
    content.style.display = (content.style.display === 'block') ? 'none' : 'block';
  }
</script>

</body>
</html>
