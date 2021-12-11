<template>
  <div class="light">
    <Header />
    <main id="main">
      <section id="mainCont2">
        <h2 class="sr-only">메인 컨텐츠 영역입니다.</h2>
        <div class="main__cont2">
          <div v-for="title in titles" v-bind:key="title.text">
            {{ title.text }}
          </div>
        </div>
        <img src="../assets/img/main_img.png" alt="이미지" />
        <div class="circle"></div>
      </section>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';

export default {
  components: {
    Header,
    Footer,
  },

  data: function () {
    return {
      titles: [{ text: 'FRONTEND VUE.JS' }, { text: 'DEVELOPER' }],
    };
  },
};
</script>

<style lang="scss">
.main__cont {
  color: #000;
  font-size: 7vw;
  line-height: 0.85;
  letter-spacing: -0.0275em;
  transition: all 2s;
  text-transform: uppercase;
  font-family: 'saol';
  margin-top: 25vw;
  .l2 {
    margin-left: 9vw;
  }
  .l3 {
    margin-left: 18vw;
  }
}
.main__cont.tact {
  div:nth-child(2) {
    margin-left: 9vw;
  }
  div:nth-child(3) {
    margin-left: 18vw;
  }
}
.light #mainCont {
  background-color: #f0eeeb;

  .main__cont {
    color: #000;
  }
}

#mainCont2 {
  background-color: #f4f1ef;
  height: 100vh;
  color: #000;
  font-family: 'saol';
  font-size: 6vw;
  text-align: center;
  line-height: 0.91;
  text-transform: uppercase;
  display: flex;
  align-items: center;
  justify-content: center;

  br {
    display: none;
  }

  .main__cont2 {
    margin-top: 450px;
  }
  img {
    width: 300px;
    z-index: 10;
    display: flex;
    position: absolute;
    margin-top: -160px;
  }
  .circle {
    width: 2050px;
    height: 2050px;
    border: 3px solid #e9e3df;
    border-radius: 50%;
    position: fixed;
    margin-top: 1700px;
    z-index: 1;
  }
}
</style>
