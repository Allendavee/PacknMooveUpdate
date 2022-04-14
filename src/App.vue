<template>
  <div class="others">
    <p>Call: 08112345678</p>
    <p>Email: info@Packnmoove.ocm.ng</p>
    <div class="social-top">
      <i class="bx bxl-twitter"></i>
      <i class="bx bxl-facebook"></i>
      <i class="bx bxl-instagram"></i>
    </div>
  </div>
  <hr class="rule" />
  <Navbar />
  <router-view />
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
  component: {
    Navbar,
  },
};
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@200;300;400;500;600;700&family=Quicksand:wght@300;400;500;600;700&family=Raleway:ital,wght@0,100;0,300;0,400;0,500;0,600;0,700;1,300&family=Roboto:ital,wght@0,100;0,300;0,500;1,100&family=Source+Sans+Pro&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@200;300;400;500;600;700&family=Quicksand:wght@300;400;500;600;700&family=Raleway:ital,wght@0,100;0,300;0,400;0,500;0,600;0,700;1,300&family=Roboto:ital,wght@0,100;0,300;0,500;1,100&family=Source+Sans+Pro:wght@300;400;600;700&display=swap');
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
  font-family: 'Source Sans Pro', sans-serif;
  /* -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; */
}
.others {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  margin: 12px 0 8.5px 0;
}
.others > p {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;

  color: #616060;
}
.others > p:nth-child(2) {
  margin: 0 55px;
}
.social-top {
  padding-right: 5%;
}
.social-top > i {
  color: #fff;
  height: 32px;
  width: 32px;
  background-color: #0187ba;
  padding: 8px;
  font-size: 16px;
  border-radius: 50%;
  margin: 0 10px;
}
hr {
  height: 0.5px;
  color: #0187ba;
  width: 100%;
  background-color: #0187ba;
  border: none;
  margin-bottom: -25px;
}
</style>
