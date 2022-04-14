<template>
  <div class="home">
    <Navbar />

    <div class="container">
      <div class="row">
        <div class="col">
          <h3>Move with Ease</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ex
            lorem, consequat id posuere ut, tincidunt scelerisque urna.
            Suspendisse eget mi fermentum, condimentum augue nec, malesuada
            justo.
          </p>
          <button class="btn">Request Quote</button>
        </div>
        <div class="col">
          <img src="@/assets/group.png" alt="" />
        </div>
      </div>
    </div>
  </div>

  <Homeservices />
</template>

<script>
import Navbar from "../components/Navbar.vue";
import Homeservices from  "../components/Homeservices.vue"
// @ is an alias to /srcimport HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  mounted() {
    document.title = "Home | Packnmoove.com.ng";
  },
  components: {
    Navbar,
    Homeservices,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@200;300;400;500;600;700&family=Quicksand:wght@300;400;500;600;700&family=Raleway:ital,wght@0,100;0,300;0,400;0,500;0,600;0,700;1,300&family=Roboto:ital,wght@0,100;0,300;0,500;1,100&family=Source+Sans+Pro:wght@300;400;600;700&display=swap");
.home {
  background-image: url("~@/assets/Vector.png");
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center;
  width: 100%;
  height: 700px;
  margin-top: 0;
}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
.row {
  display: flex;
  justify-content: center;
  align-items: center;
}
.col {
  flex-basis: 48%;
}
.col > img {
  width: 600px;
}
.col > p {
  width: 541px;
  font-family: "Source Sans Pro", sans-serif;
  font-style: normal;
  font-weight: 300px;
  font-size: 18px;
  line-height: 23px;
  color: #1d1d1b;
  margin-bottom: 24px;
  

}
.col > h3 {
  font-family: "Inter", sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 64px;
  line-height: 77px;
  color: #219bc2;
  margin-bottom: 24px;
}
.btn {
  border: none;
  background: #ea9a27;
  border-radius: 10px;
  padding: 12px 36px;
  font-size: 20px;
  line-height: 25px;
  color: #ffffff;
  cursor: pointer;
}
</style>
