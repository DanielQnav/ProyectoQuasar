<template>
<div class="flex flex-center bg-blue">
      <img class="q-pa-lg" src="~assets/quasar-logo-vertical.svg" alt="Web desing" height="100" width="100">
    </div>
  <q-page>
    <div class="row">
      <div class="col bg-blue shadow-10 ">
        <h3 class="text-dark text-center text-weight-bold">Actividad Quasar</h3>
      </div>
    </div>
    <div class="flex flex-center">
      <img class="q-pa-lg" src="~assets/quasar-logo-vertical.svg" alt="Web desing" height="300" width="400">
    </div>
    <div class="row justify-center">
      <div class="col-6">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius ad sed placeat maxime distinctio. Commodi inventore voluptatibus quas architecto, porro, aliquam quae itaque nobis blanditiis exercitationem alias tempora impedit laboriosam!
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius ad sed placeat maxime distinctio. Commodi inventore voluptatibus quas architecto, porro, aliquam quae itaque nobis blanditiis exercitationem alias tempora impedit laboriosam!
        </p>
      </div>
    </div>
    
    <div class="row q-py-xl" >
      
      <div class="row justify-center bg-blue-13 q-py-md shadow-10 bordes-redon">
        <div class="col text-center contendor">
          <h5 class="text-dark text-weight-bold">Lorem</h5>
          <p class="text-left q-mx-md text-dark">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
        <div class="col text-center contendor">
          <h5 class="text-dark text-weight-bold">Lorem</h5>
          <p class="text-left q-mx-md text-dark">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
        <div class="col text-center contendor">
          
          <h5 class="text-dark text-weight-bold">Lorem</h5>
          <p class="text-left q-mx-md text-dark">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
        <div class="col text-center contendor">
          <h5 class="text-dark text-weight-bold">Lorem</h5>
          <p class="text-left q-mx-md text-dark">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, animi corrupti! Autem modi animi incidunt nihil ipsa, odio ullam. Odio porro, exercitationem dolor natus repellat numquam beatae dolorum illo sint?</p>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'PageIndex'
})
</script>

<style lang="scss" scoped>
.bordes-redon{
  border-radius: 20px;
}
.mover{
  position: relative;
  transform: translateY(-25px);
  z-index: 1;
  font-size: 70px;
  height: 0;
}
.contenedor{
  position: absolute;
  z-index: 0;
}
</style>