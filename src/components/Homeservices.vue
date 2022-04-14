<template>
  <div class="grid">
    <div class="container-item item1">
      <h5>
        Our Services
      </h5>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ex lorem, consequat id posuere ut, tincidunt scelerisque urna. Suspendisse eget mi fermentum, condimentum augue nec, malesuada justo. Lorem ipsum  
      </p>
    </div>
    <div class="container-item bar">
      <img src="@/assets/home.png" alt="" />
      <h5>Home</h5>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    <div class="container-item bar">
      <img src="@/assets/office.png" alt="" />
      <h5>Office</h5>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    <div class="container-item bar">
      <img src="@/assets/interstate.png" alt="" />
      <h5>Inter-state</h5>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    <div class="container-item bar">
      <img src="@/assets/installation.png" alt="" />
      <h5>Installation</h5>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    <div class="container-item bar">
      <img src="@/assets/home.png" alt="" />
      <h5>Cleaning & Packing</h5>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    <div class="container-item bar">
      <img src="@/assets/home.png" alt="" />
      <h5>Equipment Moves</h5>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.grid {
  display: grid;
  padding: 70px 130px;
  grid-template-columns: repeat(4, 1fr);
  column-gap: 16px;
  row-gap: 16px;

  background-color: #f1fbff;
}
.container-item {
  background-color: #fff;
  padding: 16px;
  /* margin-bottom: 16px; */
  border-radius: 10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.bar {
  background-image: url("~@/assets/bar.png");
  background-size: contain;
  background-repeat: no-repeat;
  background-position: bottom;

  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
}
.item1{
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-direction: column;
}
.bar p {
  text-align: center;
  font-weight: 300;
  font-size: 16px;
  line-height: 20px;
  text-align: center;
  color: #3d3c3c;
}
.item1 p {
  text-align: center;
  font-weight: 300;
  font-size: 16px;
  line-height: 20px;
  text-align: center;
  color: #3d3c3c;
}
.bar h5 {
  font-weight: 600;
  font-size: 18px;
  line-height: 24px;
  color: #219bc2;
  padding-top: 8px;
}
.item1 h5 {
  font-weight: 600;
  font-size: 18px;
  line-height: 24px;
  color: #219bc2;
  padding-top: 8px;
}
.bar > img {
  height: 65px;
  width: 65px;
}
.item1 {
  grid-row: 1 / span 2;
  background-image: url("~@/assets/barrect.png");
  background-size: contain;
  background-repeat: no-repeat;
  background-position: left;
}
</style>