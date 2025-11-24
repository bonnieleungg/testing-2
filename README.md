# YF AIPO testing-2 
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>YouFind AI SEO 平台</title>
  <style>
    /* Reset 與基礎樣式 */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "PingFang TC",
        "Microsoft JhengHei", sans-serif;
      background-color: #ffffff;
      color: #000000;
      line-height: 1.6;
    }
    a {
      color: #000000;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }

    /* Header 與導覽列 */
    header {
      background: #000000;
      color: #ffffff;
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      font-weight: bold;
      font-size: 1.4rem;
      letter-spacing: 2px;
      cursor: default;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 1.5rem;
    }
    nav ul li a {
      color: #ffffff;
      font-weight: 600;
      font-size: 0.95rem;
      padding: 0.5rem 0;
      display: inline-block;
    }

    /* 手機版漢堡選單 */
    .menu-toggle {
      display: none;
      flex-direction: column;
      cursor: pointer;
      gap: 5px;
    }
    .menu-toggle span {
      width: 24px;
      height: 3px;
      background: #ffffff;
      display: block;
      border-radius: 1px;
    }

    @media (max-width: 768px) {
      nav ul {
        position: absolute;
        top: 60px;
        right: 0;
        background: #000000;
        width: 220px;
        flex-direction: column;
        border-radius: 4px;
        display: none;
        padding: 1rem;
      }
      nav ul.show {
        display: flex;
      }
      .menu-toggle {
        display: flex;
      }
    }

    /* 主內容區 */
    main {
      max-width: 1100px;
      margin: 2rem auto;
      padding: 0 1rem;
    }
    section {
      margin-bottom: 4rem;
    }
    h1, h2, h3 {
      margin-bottom: 1rem;
      font-weight: 700;
    }
    h1 {
      font-size: 2.2rem;
      letter-spacing: 2px;
      text-align: center;
      margin-bottom: 2rem;
    }
    h2 {
      font-size: 1.8rem;
      border-bottom: 2px solid #000000;
      padding-bottom: 0.4rem;
    }
    h3 {
      font-size: 1.2rem;
    }
    p {
      margin: 0.6rem 0 1.2rem;
      font-size: 1rem;
    }

    /* 影片與圖片容器 */
    .video-container,
    .image-container {
      max-width: 100%;
      margin: 1rem 0;
      text-align: center;
    }
    iframe, img {
      max-width: 100%;
      height: auto;
      border: none;
    }

    /* 方案區塊 */
    .plans {
      display: flex;
      gap: 2rem;
      flex-wrap: wrap;
      justify-content: center;
    }
    .plan {
      border: 1px solid #000000;
      border-radius: 6px;
      padding: 1.5rem;
      width: 280px;
      background: #f8f8f8;
      color: #000000;
      text-align: center;
      transition: box-shadow 0.3s ease;
    }
    .plan:hover {
      box-shadow: 0 0 10px #000000;
    }
    .plan h3 {
      margin-bottom: 0.5rem;
    }
    .plan p.price {
      font-size: 1.5rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }
    .plan ul {
      list-style: none;
      margin-bottom: 1rem;
      text-align: left;
    }
    .plan ul li {
      padding: 0.3rem 0;
      border-bottom: 1px solid #dddddd;
      font-size: 0.95rem;
    }
    .plan button {
      background: #000000;
      color: #ffffff;
      border: none;
      padding: 0.8rem 1.5rem;
      cursor: pointer;
      border-radius: 4px;
      font-weight: 600;
      transition: background-color 0.3s ease;
    }
    .plan button:hover {
      background: #444444;
    }

    /* Blog 區塊 */
    .blog-posts {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }
    .post {
      border: 1px solid #000000;
      padding: 1rem;
      border-radius: 4px;
      background: #f8f8f8;
      color: #000000;
    }
    .post h3 {
      margin-bottom: 0.8rem;
    }

    /* Footer */
    footer {
      background: #000000;
      color: #ffffff;
      text-align: center;
      padding: 1.5rem 1rem;
      font-size: 0.85rem;
      letter-spacing: 1px;
      margin-top: 4rem;
    }
    footer a {
      color: #ffffff;
      text-decoration: underline;
      font-weight: 600;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">YouFind AI SEO</div>
    <div class="menu-toggle" id="menu-toggle" aria-label="開啟選單" role="button" tabindex="0">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <nav>
      <ul id="nav-links">
        <li><a href="#why-matters">為何這很重要</a></li>
        <li><a href="#ai-overview">AI 總覽</a></li>
        <li><a href="#seo-aipo">SEO AIPO</a></li>
        <li><a href="#search-visibility">搜尋能見度雲</a></li>
        <li><a href="#plans">方案與收費</a></li>
        <li><a href="#full-funnel">全漏斗成長</a></li>
        <li><a href="#blog">GEO 部落格</a></li>
        <li><a href="#contact">聯絡我們</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <!-- 為何這很重要 -->
    <section id="why-matters">
      <h1>為何 AI 搜尋能見度這麼重要？</h1>
      <p>
        在 AI 主導的搜尋時代，品牌不只要在 Google 傳統搜尋結果出現，更要在
        AI Overview、ChatGPT、Perplexity 等生成式搜尋答案中被看見，否則就算你在
        SEO 排名不錯，依然會在 AI 回覆裡「消失」。
      </p>
      <p>
        YouFind 的 GEO / AIPO 框架，協助企業把內容轉化為 AI 友善的結構化訊號，
        在各種 AI 搜尋介面中維持穩定的曝光與權威敘事。
      </p>
    </section>

    <!-- AI 總覽 -->
    <section id="ai-overview">
      <h2>Google AI Overview 簡介</h2>
      <div class="video-container">
        <!-- 這裡用示意影片 URL，你可以換成自己真正的影片嵌入 -->
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/DAG5Aggs3b0"
          title="Google AI Overview 示意影片"
          frameborder="0"
          allowfullscreen>
        </iframe>
      </div>
      <p>
        AI Overview 將傳統 SEO 結果重新包裝成一段整合式的 AI 回應，引用不同網站的內容作為來源；
        如果沒有針對 AI 結構化與敘事佈局，品牌就算有排名，也很容易被其他更「AI 就緒」的內容取代。
      </p>
      <p>
        YouFind 會從關鍵查詢、Schema、FAQ、比較頁等角度，設計完整的 AI 搜尋能見度策略，
        確保品牌在 AI 回應中獲得正確、突出且可被點擊的展示。
      </p>
    </section>

    <!-- SEO AIPO -->
    <section id="seo-aipo">
      <h2>SEO AIPO：AI 搜尋優化新框架</h2>
      <p>
        AIPO（AI Platform Optimization）是延伸自傳統 SEO 的新一代框架，
        不只看 Google 排名，更關注在各種 AI 平台（Google AI Overview、ChatGPT、
        Perplexity、Bing Copilot 等）上的曝光、引用與敘事權。
      </p>
      <p>
        我們會依據核心主題，規劃 FAQ 頁、比較頁、資料頁與部落格集群，配合結構化標記與
        Topic Cluster，讓 AI 能夠更精準理解你的品牌定位與專業範疇。
      </p>
      <div class="image-container">
        <!-- 示意圖片，可替換為實際設計圖 -->
        <img
          src="https://via.placeholder.com/800x400?text=SEO+AIPO+Illustration"
          alt="SEO AIPO AI 搜尋示意圖" />
      </div>
    </section>

    <!-- 搜尋能見度雲 -->
    <section id="search-visibility">
      <h2>YouFind Search Visibility Cloud</h2>
      <p>
        Search Visibility Cloud 是 YouFind 的搜尋能見度雲端平台，整合超過 20 組
        SEO 與第三方數據資產，從關鍵字、排名、AI 回應引用來源到第三方口碑訊號，
        一站式呈現你的「搜尋與 AI 能見度」全貌。
      </p>
      <p>
        透過 AIPO Score 與 Query Engine，你可以清楚看到品牌在不同查詢、不同平台、
        不同階段（ZMOT、UMOT）下的表現，並獲得具體的優化建議。
      </p>
    </section>

    <!-- 方案與收費 -->
    <section id="plans">
      <h2>方案與收費</h2>
      <div class="plans">
        <div class="plan">
          <h3>方案一：Pure AIPO</h3>
          <ul>
            <li>AIO / AI 能見度稽核</li>
            <li>10–20 組核心 FAQ 與查詢群組規劃</li>
            <li>AI 可爬行度與 Schema 檢查</li>
            <li>AI Overview 追蹤與報告</li>
          </ul>
          <button>了解 Pure AIPO</button>
        </div>

        <div class="plan">
          <h3>方案二：On-going AIPO</h3>
          <ul>
            <li>持續 6–12 個月 AI 搜尋優化</li>
            <li>20–40 組 FAQ / 查詢群組擴展</li>
            <li>AI Recommendation 與 Schema 持續優化</li>
            <li>定期 Benchmark 與競品差距分析</li>
          </ul>
          <button>了解 On-going AIPO</button>
        </div>

        <div class="plan">
          <h3>方案三：SEO + AIPO</h3>
          <ul>
            <li>完整 SEO + AIPO 雙軌策略</li>
            <li>Topic Cluster 建構與舊內容重寫</li>
            <li>排名與 AI 能見度雙 KPI 追蹤</li>
            <li>持續內容刷新與成長報告</li>
          </ul>
          <button>了解 SEO + AIPO</button>
        </div>

        <div class="plan">
          <h3>方案四：SEO + AIPO + UMOT</h3>
          <ul>
            <li>從 Zero Moment 到 Ultimate Moment 全漏斗布局</li>
            <li>社群聲量與公共關注議題監測</li>
            <li>敘事角度設計與信任訊號佈局</li>
            <li>第三方平台與口碑分發管理</li>
          </ul>
          <button>了解 Full Funnel</button>
        </div>
      </div>
    </section>

    <!-- 全漏斗成長 -->
    <section id="full-funnel">
      <h2>Full Funnel Growth：全漏斗成長引擎</h2>
      <p>
        YouFind 將 Paid Media、SEO、AIPO 與 UMOT 結合，從搜尋觸發、
        評估比較、決策轉換，到購買後的口碑與再行銷，建立一條完整的
        Full Funnel Growth Engine。
      </p>
      <p>
        透過年對年的成效承諾（例如曝光、點擊、轉換與 AI 能見度成長），
        讓行銷預算在 AI 搜尋時代不只「被看見」，更能驅動實際生意成果。
      </p>
    </section>

    <!-- GEO Blog 區 -->
    <section id="blog">
      <h2>GEO 部落格</h2>
      <div class="blog-posts">
        <article class="post">
          <h3>GEO 是什麼？為何在 AI 時代更關鍵？</h3>
          <p>
            GEO（Search & AI Visibility for GEO Keywords）強調以「地標、品牌、品類」
            等關鍵詞為主軸，確保你的品牌在使用者所有與地理、品類相關的查詢——
            包括 AI 聊天與 AI Overview 裡——都能被正確提及與引用。
          </p>
        </article>

        <article class="post">
          <h3>案例：排名第 2，卻在 AI 回覆中消失</h3>
          <p>
            以「mba hk」為例，即使某商學院在 Google 自然排序中名列前茅，但當使用者在
            Perplexity 問「香港最好的商學院是什麼？」時，AI 回覆只列出其他院校，
            該品牌完全沒有出現在答案裡。
          </p>
        </article>

        <article class="post">
          <h3>從 SEO 到 AIPO：你的內容準備好了嗎？</h3>
          <p>
            傳統 SEO 重視頁面與關鍵字；AIPO 則把重心拉到「查詢意圖、敘事與結構化數據」，
            讓 AI 願意且能夠引用你的內容。這需要從內容架構到技術實作的全面調整。
          </p>
        </article>
      </div>
    </section>

    <!-- 聯絡我們 -->
    <section id="contact">
      <h2>聯絡我們</h2>
      <p>如需了解 GEO / AIPO 或客製方案，歡迎直接與我們聯繫：</p>
      <p>Email：<a href="mailto:sales@youfind.com">sales@youfind.com</a></p>
      <p>電話：+852 0000 0000（示意）</p>
      <p>地址：香港 ·（此處可填寫實際公司地址）</p>
    </section>
  </main>

  <footer>
    <p>© 2025 YouFind GEO / AIPO Search Visibility | <a href="#contact">聯絡我們</a></p>
  </footer>

  <script>
    // 手機版選單切換
    const menuToggle = document.getElementById('menu-toggle');
    const navLinks = document.getElementById('nav-links');

    menuToggle.addEventListener('click', function () {
      navLinks.classList.toggle('show');
    });

    // 點選連結後收起選單（手機）
    navLinks.addEventListener('click', function (e) {
      if (e.target.tagName === 'A') {
        navLinks.classList.remove('show');
      }
    });
  </script>
</body>
</html>
