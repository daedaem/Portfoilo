<template>
  <div class="total-frame">
    <div class="total-info-box">
      <div class="image-box">
        <!-- <img class="profile-image" src="@/assets/profileImage.jpg" alt="" /> -->
        <!-- <img class="profile-image" src="@/assets/motorcycleAndMe.jpg" alt="" /> -->
        <img class="profile-image" src="@/assets/profileImage.jpg" alt="" />
      </div>
      <div class="info-box col-6">
        <!-- <h1 class="mb-4">Haesung Cho</h1> -->
        <!-- <h5 class="mb-2">Frontend Developer.</h5> -->
        <div class="introduction-content">
          석사과정에서 IBM사의 AI 신약후보물질을 찾을 수 있는 '왓슨' 플랫폼
          사용경험은 개발 직무에 대한 꿈을 갖게 해준 계기가 되었습니다.
          <br />
          개발자는 인류가 직면한 문제를 해결 할 수 있다고 믿습니다.
          <br />
          결국 해내는 집념을 갖고 있는 프론트엔드 개발자 조해성입니다.
        </div>
        <!-- <p>
        I believe developers are people who can solve the problems that humans
        are experiencing.
      </p> -->
        <div class="subinfo-box">
          <div>
            <p><strong> E-mail</strong> : tg8685@gmail.com</p>
          </div>
          <div>
            <p><strong> Phone</strong> : +82 10-4449-8685</p>
          </div>
          <div>
            <p><strong> City</strong> : 부산, 대한민국</p>
          </div>
        </div>
        <div
          class="d-flex justify-content-start align-items-center link-images"
        >
          <a :href="links.facebook" target="_blank">
            <img
              class="link-image"
              src="@/assets/facebook-square-brands.svg"
              alt=""
          /></a>
          <a :href="links.github" target="_blank"
            ><img
              class="link-image"
              src="@/assets/github-square-brands.svg"
              alt=""
          /></a>
          <a :href="links.instagram" target="_blank"
            ><img
              class="link-image"
              src="@/assets/instagram-square-brands.svg"
              alt=""
          /></a>
          <a :href="links.linkedin" target="_blank"
            ><img class="link-image" src="@/assets/linkedin-brands.svg" alt=""
          /></a>
        </div>
      </div>
      <div class="col d-flex justify-content-center"></div>
    </div>
    <div class="accordion" id="accordionPanelsStayOpenExample">
      <div class="accordion-item">
        <h2 class="accordion-header" id="panelsStayOpen-headingOne">
          <button
            class="accordion-button"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#panelsStayOpen-collapseOne"
            aria-expanded="true"
            aria-controls="panelsStayOpen-collapseOne"
          >
            Accordion Item #1
          </button>
        </h2>
        <div
          id="panelsStayOpen-collapseOne"
          class="accordion-collapse collapse show"
          aria-labelledby="panelsStayOpen-headingOne"
        >
          <div class="accordion-body">
            <strong>This is the first item's accordion body.</strong> It is
            shown by default, until the collapse plugin adds the appropriate
            classes that we use to style each element. These classes control the
            overall appearance, as well as the showing and hiding via CSS
            transitions. You can modify any of this with custom CSS or
            overriding our default variables. It's also worth noting that just
            about any HTML can go within the <code>.accordion-body</code>,
            though the transition does limit overflow.
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="accordion-header" id="panelsStayOpen-headingTwo">
          <button
            class="accordion-button collapsed"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#panelsStayOpen-collapseTwo"
            aria-expanded="false"
            aria-controls="panelsStayOpen-collapseTwo"
          >
            Accordion Item #2
          </button>
        </h2>
        <div
          id="panelsStayOpen-collapseTwo"
          class="accordion-collapse collapse"
          aria-labelledby="panelsStayOpen-headingTwo"
        >
          <div class="accordion-body">
            <strong>This is the second item's accordion body.</strong> It is
            hidden by default, until the collapse plugin adds the appropriate
            classes that we use to style each element. These classes control the
            overall appearance, as well as the showing and hiding via CSS
            transitions. You can modify any of this with custom CSS or
            overriding our default variables. It's also worth noting that just
            about any HTML can go within the <code>.accordion-body</code>,
            though the transition does limit overflow.
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="accordion-header" id="panelsStayOpen-headingThree">
          <button
            class="accordion-button collapsed"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#panelsStayOpen-collapseThree"
            aria-expanded="false"
            aria-controls="panelsStayOpen-collapseThree"
          >
            Accordion Item #3
          </button>
        </h2>
        <div
          id="panelsStayOpen-collapseThree"
          class="accordion-collapse collapse"
          aria-labelledby="panelsStayOpen-headingThree"
        >
          <div class="accordion-body">
            <strong>This is the third item's accordion body.</strong> It is
            hidden by default, until the collapse plugin adds the appropriate
            classes that we use to style each element. These classes control the
            overall appearance, as well as the showing and hiding via CSS
            transitions. You can modify any of this with custom CSS or
            overriding our default variables. It's also worth noting that just
            about any HTML can go within the <code>.accordion-body</code>,
            though the transition does limit overflow.
          </div>
        </div>
      </div>
    </div>
    <ETC></ETC>
  </div>
</template>
<script>
import { reactive } from "vue";
import ETC from "./ETC.vue";
export default {
  name: "About",
  components: { ETC },
  setup() {
    const links = reactive({
      facebook: "https://www.facebook.com/tanggae",
      github: "https://github.com/daedaem",
      instagram: "https://www.instagram.com/sun_castle_8685/",
      linkedin:
        "https://www.linkedin.com/in/%ED%95%B4%EC%84%B1-%EC%A1%B0-518a021a9/",
    });
    return { links };
  },
};
</script>
<style lang="scss">
h1 {
  font-size: 4rem;
  font-weight: bold;
  font-family: "SF Pro Display", -apple-system, system-ui, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}
h2 {
  font-size: 3.5rem;
}
h3 {
  font-size: 3rem;
  font-weight: bold;
  font-family: "SF Pro Display", -apple-system, system-ui, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}
h4 {
  font-size: 2rem;
}
h5 {
  font-size: 1.5rem;
}
a {
  color: black;
  // font-size: 1rem;
  text-decoration: none;
}

.total-info-box {
  max-width: 1000px;
  height: 94vh;
  margin: 0rem auto 0rem auto;
  display: flex;
  align-items: center;
}
.info-box {
  text-align: start;
  padding: 0rem 0rem 0rem 3rem;
  // background: #fafafa;
}
.introduction-content {
  text-align: start;
  // align-items: center;
  // padding: 1rem 4rem 1rem 1rem;
}
.subinfo-box {
  margin: 2rem 0rem 0rem 0rem;
}

.image-box {
  // background: whitesmoke;
  // align-items: center;
  width: 350px;
  height: 350px;

  border-radius: 100%;
  overflow: hidden;
  // width: 400px;
}
.profile-image {
  object-fit: cover;
  width: 100%;
  height: 100%;

  // width: 400px;
}
.link-images {
  gap: 1rem;
}
.link-image {
  width: 2rem;
}
.accordion {
  max-width: 1000px;
  margin: auto;
}
</style>
