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

    <!-- box menu Dessert -->
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
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/menu.scss';
</style>