<template>
<section class="works" id="Works">
  <div class="text">
    <h1>Works</h1>
    <h2>たとえば何作ってんすか？</h2>
  </div>
  <div class="scroll_wrap">
    <div class="scroll_track js-scrollTrack">
      <ul class="scroll_inner js-scrollList">
        <li class="scroll_cont js-scrollCont">
          <img src="../assets/testpic_2.png" alt="taiki">
          <h1>ああ 良き天気</h1>
          <p>本学で最も無意味な動画です</p>
        </li>
        <li class="scroll_cont js-scrollCont">
          <img src="../assets/testpic_1.png" alt="taiki">
          <h1>心安らかなり 日本の夏 蝉の声</h1>
          <p>雪だるま作ろう</p>
        </li>
        <li class="scroll_cont js-scrollCont">
          <img src="../assets/testpic_2.png" alt="taiki">
          <h1>いま静かにして</h1>
          <p>木の下に宿れるなり</p>
        </li>
        <li class="scroll_cont js-scrollCont">
          <img src="../assets/testpic_1.png" alt="taiki">
          <h1>我が心 その宿れるなりと同じき</h1>
        </li>
        <li class="scroll_cont js-scrollCont">
          <img src="../assets/testpic_2.png" alt="taiki">
          <h1>安き心にある</h1>
        </li>
      </ul>
    </div>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceWorks'
}

const infiniteScroller = (target, options) => {
  const defaultOptions = {
    clones: 1,
    direction: "left",
    duration: "20s",
    pauseOnHover: true
  };
  const scrollOptions = { ...defaultOptions, ...options };

  const body = document.body;
  const scrollTarget = target || document.querySelector(".js-scrollTrack");
  const scrollList = scrollTarget.querySelector(".js-scrollList");
  const scrollCont = scrollTarget.querySelectorAll(".js-scrollCont");
  const cloneLength = scrollOptions.clones + 1;

  const init = () => {
    scrollTarget.setAttribute("data-scroll-initialized", "true");
    body.style.setProperty(
      "--_infinite-scroll-clone-length",
      cloneLength.toString()
    );

    scrollOptions.direction === "left"
      ? scrollTarget.setAttribute("data-scroll-direction", "left")
      : scrollTarget.setAttribute("data-scroll-direction", "right");

    if (scrollOptions.pauseOnHover)
      scrollTarget.setAttribute("data-scroll-pause-on-hover", "true");

    if (scrollOptions.gap)
      body.style.setProperty("--_infinite-scroll-gap", scrollOptions.gap);
    if (scrollOptions.duration)
      body.style.setProperty(
        "--_infinite-scroll-duration",
        scrollOptions.duration
      );

    for (let i = 0; i < scrollOptions.clones; i++) {
      scrollCont.forEach((element) => {
        const duplicatedItem = element.cloneNode(true);
        duplicatedItem.setAttribute("aria-hidden", "true");
        scrollList
          ? scrollList.appendChild(duplicatedItem)
          : scrollTarget.appendChild(duplicatedItem);
      });
    }
  };

  init();
};

window.addEventListener("DOMContentLoaded", () => {
  const scrollTarget = document.querySelector(".js-scrollTrack");
  if (!scrollTarget) return;

  infiniteScroller(scrollTarget, {
    clones: 1,
    gap: "30px"
  });
});
</script>

<style scoped>
section{
  width: 100%;
  height: 600px;
  background: #ffffff;
  position: relative;
}
.text {
  width: 50%;
  text-align: left;
  position: absolute;
  top: 5%;
  left: 18%;
  margin: 0;
  padding: 0;
}
.text h1 {
  font-size: 3rem;
  color: black;
  margin-bottom: 0;
}
.text h2 {
  font-size: 1.8rem;
  color: #314F87;
  margin-top: 0;
}

/* スクロールされるコンテンツ郡について */
.scroll_wrap {
  margin-block-start: 20vh;
  width: 100%;
  overflow: hidden;
}

.scroll_cont {
  display: flexbox; /* flexboxとgridどっちでも動くけど見た目変わる */
  place-content: top;
  flex-shrink: 0;
  width: 35vw;
  overflow: hidden;
  aspect-ratio: 5 / 4;
  border-radius: 10px;
  color: white;
  border: 1px solid #b3b3b3;
  filter: drop-shadow(0px 0px 3px #a3a3a3);
  &:nth-of-type(n) {
    background-color: #f3f3f3;
  }
}

.scroll_cont img {
  width: 35vw;
  border-radius: 10px 10px 0px 0px;
}

.scroll_cont h1 {
  font-size: 1rem;
  font-weight: bold;
  color: #000000;
  padding: 0rem 1rem;
  margin-bottom: 0;
}

.scroll_cont p {
  font-size: 0.8rem;
  color: #000000;
  padding: 0rem 1rem;
  margin-top: 0;
}

@keyframes infiniteScrollRTL {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(
      calc(
        -1 * (100% / var(--_infinite-scroll-clone-length)) - var(
            --_infinite-scroll-gap,
            var(--scroll-gap)
          ) / var(--_infinite-scroll-clone-length)
      )
    );
  }
}

@keyframes infiniteScrollLTR {
  0% {
    transform: translateX(
      calc(
        -1 * (100% / var(--_infinite-scroll-clone-length)) - var(
            --_infinite-scroll-gap,
            var(--scroll-gap)
          ) / var(--_infinite-scroll-clone-length)
      )
    );
  }
  100% {
    transform: translateX(0);
  }
}

.js-scrollTrack {
  width: max-content;

  &[data-scroll-initialized="true"][data-scroll-direction="left"] {
    animation: infiniteScrollRTL var(--_infinite-scroll-duration) linear
      infinite;
  }
  &[data-scroll-initialized="true"][data-scroll-direction="right"] {
    animation: infiniteScrollLTR var(--_infinite-scroll-duration) linear
      infinite;
  }
  &[data-scroll-pause-on-hover="true"]:hover {
    animation-play-state: paused;
  }
}

.js-scrollList {
  display: flex;
  flex-wrap: nowrap;
  gap: 0 var(--_infinite-scroll-gap, var(--scroll-gap));
}

.js-scrollCont {
  flex-shrink: 0;
}

</style>