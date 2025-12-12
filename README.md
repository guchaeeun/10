<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>나만의 힐링송 소개하기</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>My Healing Power-Up Songs</h1>
    <p>기분이 안 좋아지거나 힘들 때, 볼륨 끝까지 올려 듣는 전투력 상승 힐링송 플레이리스트</p>
  </header>

  <nav>
    <button class="tab" data-category="breakup">이별할 때</button>
    <button class="tab" data-category="walk">산책할 때</button>
    <button class="tab" data-category="snow">눈 올 때</button>
    <button class="tab" data-category="hot">더울 때</button>
  </nav>

  <main>
    <!-- 이별할 때 -->
    <section id="breakup" class="category-section">
      <article>
        <a href="https://www.youtube.com/watch?v=jT27daayn_k" target="_blank">
          <img src="KakaoTalk_20251212_124600178.jpg" alt="임한별 - 이별하러 가는 길" />
          <h3>임한별 - 이별하러 가는 길</h3>
        </a>
      </article>
      <article>
        <a href="https://www.youtube.com/watch?v=hrO-BgLjJ-Q" target="_blank">
          <img src="KakaoTalk_20251212_124600178_01.jpg" alt="윤하 - 먹구름" />
          <h3>윤하 - 먹구름</h3>
        </a>
      </article>
      <article>
        <a href="https://www.youtube.com/watch?v=EUFSDbnZ1o4" target="_blank">
          <img src="KakaoTalk_20251212_124600178_02.jpg" alt="토이(with 권진아) - 그녀가 말했다" />
          <h3>토이(with 권진아) - 그녀가 말했다</h3>
        </a>
      </article>
    </section>

    <!-- 산책할 때 -->
    <section id="walk" class="category-section" style="display:none;">
      <article>
        <a href="https://youtu.be/nej08HFsp7A?si=Tov7dcVonLm9Kr5u" target="_blank">
          <img src="KakaoTalk_20251212_124710953.jpg" alt="Big void - 실리카겔" />
          <h3>Big void - 실리카겔</h3>
        </a>
      </article>
      <article>
        <a href="https://youtu.be/iAeeTin1uCA?si=fpSF4_TIh3qMzKOe" target="_blank">
          <img src="KakaoTalk_20251212_124710953_01.jpg" alt="산책 - 백예린" />
          <h3>산책 - 백예린</h3>
        </a>
      </article>
      <article>
        <a href="https://youtu.be/t54PzeNJDIA?si=nkDX7gsyC1DaFBEZ" target="_blank">
          <img src="KakaoTalk_20251212_124710953_02.jpg" alt="wish - 오월오일" />
          <h3>wish - 오월오일</h3>
        </a>
      </article>
    </section>

    <!-- 눈 올 때 -->
    <section id="snow" class="category-section" style="display:none;">
      <article>
        <a href="https://www.youtube.com/watch?v=5ZB9JLfIw_Q" target="_blank">
          <img src="KakaoTalk_20251212_124725297.jpg" alt="하얀 그리움 - 프로미스나인" />
          <h3>하얀 그리움 - 프로미스나인</h3>
        </a>
      </article>
      <article>
        <a href="https://www.youtube.com/watch?v=a5oeNwoCi-s" target="_blank">
          <img src="KakaoTalk_20251212_124725297_01.jpg" alt="듣는 편지 - 40" />
          <h3>듣는 편지 - 40</h3>
        </a>
      </article>
      <article>
        <a href="https://www.youtube.com/watch?v=tnAxZipkuWw" target="_blank">
          <img src="KakaoTalk_20251212_124725297_02.jpg" alt="회전목마 - 소코도모" />
          <h3>회전목마 - 소코도모</h3>
        </a>
      </article>
    </section>

    <!-- 더울 때 -->
    <section id="hot" class="category-section" style="display:none;">
      <article>
        <a href="https://youtu.be/UDyPp9bkfD0?si=tShEXAhaPxSsnRFU" target="_blank">
          <img src="KakaoTalk_20251212_124752114.jpg" alt="DPR LIVE - Martini Blue" />
          <h3>DPR LIVE - Martini Blue</h3>
        </a>
      </article>
      <article>
        <a href="https://youtu.be/9OXAoESmsRE?si=xl0RQ_lydFCKRzxy" target="_blank">
          <img src="KakaoTalk_20251212_124752114_01.jpg" alt="투모로우바이투게더 - 그냥 괴물을 살려두면 안 되는 걸까?" />
          <h3>투모로우바이투게더 - 그냥 괴물을 살려두면 안 되는 걸까?</h3>
        </a>
      </article>
      <article>
        <a href="https://youtu.be/eG90LtY98yg?si=6agkxSM5dLPJN-_W" target="_blank">
          <img src="KakaoTalk_20251212_124752114_02.jpg" alt="샵 - sweety" />
          <h3>샵 - sweety</h3>
        </a>
      </article>
    </section>
  </main>

  <footer>
    <p>문의: youdh041009@gmail.com</p>
  </footer>

  <script>
    // 탭 버튼 클릭 시 섹션 보여주기
    const tabs = document.querySelectorAll('nav .tab');
    const sections = document.querySelectorAll('.category-section');

    tabs.forEach(tab => {
      tab.addEventListener('click', () => {
        const target = tab.getAttribute('data-category');
        sections.forEach(section => {
          section.style.display = (section.id === target) ? 'block' : 'none';
        });
      });
    });
  </script>
</body>
</html>
