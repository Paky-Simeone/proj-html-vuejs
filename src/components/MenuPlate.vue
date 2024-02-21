<script>
export default{
    data(){
        return{

        }
    },
    props:{
        firstList: Array,
        mainCourseList: Array,
        dessertList: Array,
    },
}
</script>

<template>
    <div id="menu" class="menu-container  d-flex justify-center">
      <!-- box menu Appetizer -->
      <div class="menu-box d-flex justify-center horse-doeuvres">
        <div class="text-center">
            <h2>HORSE D'OEUVRES</h2>
            <div v-for="(plate, i) in firstList" :key="i">
              <div class="menu-item d-flex space-between">
                <h3>{{ plate.plateName }}</h3>
                <span>{{ plate.price }}</span>
              </div>
              <p>{{ plate.text }}</p>
            </div>
        </div>
      </div>

      <!-- box menu MainCourse -->
      <div class="menu-box d-flex justify-center main-course">
        <div class="text-center">
            <h2>MAIN COURSE</h2>
            <div v-for="(plate, i) in mainCourseList" :key="i">
              <div class="menu-item d-flex space-between">
                <h3>{{ plate.plateName }}</h3>
                <span>{{ plate.price }}</span>
              </div>
              <p>{{ plate.text }}</p>
            </div>
        </div>
      </div>

    <!-- box menu Dessert-->
      <div class="menu-box d-flex justify-center dessert">
        <div class="text-center">
            <h2>DESSERTS</h2>
            <div v-for="(plate, i) in dessertList" :key="i">
              <div class="menu-item d-flex space-between">
                <h3>{{ plate.plateName }}</h3>
                <span>{{ plate.price }}</span>
              </div>
              <p>{{ plate.text }}</p>
            </div>
        </div>
      </div>
    </div>

    <div class="menu-jumbo" style="{  }">
      <div class="plate-back">
        <div class="plate-description justify-center">
          <div class="plate-text">
            <div class="plate">
              <h2>BRAISED <br/> ABALONE</h2>
              <span>$52</span>
            </div>
            <div class="line"></div>
            <p>Pretium accumsan porttitor viverra leo <br/> gravida mollis imperdiet. Fringilla nibh <br/> pharetra sociis leo amet.</p>
            <button class="buttonmenu">VIEW IN THE MENU</button>
          </div>
        </div>
      </div>
    </div>

</template>

<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/menu.scss';
.menu-jumbo {
  position: relative;
  width: 100%;
  height: 800px;
  background-repeat: no-repeat;
  background-position: 50%;
  background-size: cover;
  display: flex;
  align-items: center;
  padding-left: 120px;
 background-image: url(../assets/img/hero42x.jpg);
  .plate-back {
    background-color: $black-color;
    position: relative;
    width: 600px;
    height: 650px;
    .plate-description {
      padding: 0 20px;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: $white-color;
      .plate-text {
        width: 360px;
        margin: 0 40px;
        .plate {
          display: flex;
          align-items: center;
          h2 {
            font-size: 70px;
            margin-top: 0;
            display: inline;
          }
          span {
            padding-bottom: 120px;
            font-size: 20px;
          }
        }
        .line {
          margin-top: 40px;
          margin-bottom: 40px;
          width: 40px;
          border-top: 1px solid $white-color;
        }
        p {
          margin-bottom: 40px;
        }
      }
    }
  }
}
</style>