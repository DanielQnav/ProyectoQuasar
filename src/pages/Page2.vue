<template>
<div class="flex flex-center bg-blue">
      <img class="q-pa-lg" src="~assets/quasar-logo-vertical.svg" alt="Web desing" height="100" width="100">
    </div>
  <q-page>
    <div class="row">
        <div class="col bg-blue shadow-10">
            <h3 class="text-dark text-center text-weight-bold">Pagina2</h3>
        </div>
    </div>
    
    <div class="row justify-center">
        <div class="col-4 q-pa-md q-gutter-md">
            <q-card class="my-card" >
                <q-img src="~assets/quasar-logo-vertical.svg">
                  <div class="absolute-bottom">
                    <div class="text-h6">Lorem</div>
                    <div class="text-subtitle2">Subtitle</div>
                  </div>
                </q-img>
                <q-card-section>Un texto</q-card-section>
                <q-card-actions class="row justify-center" >
                  <q-btn flat glossy @click="alerta = true">Más Información</q-btn>
                </q-card-actions>
            </q-card>
        </div>
        <div class="col-4 q-pa-md q-gutter-md">
            <q-card class="my-card" >
                <q-img src="~assets/quasar-logo-vertical.svg">
                  <div class="absolute-bottom">
                    <div class="text-h6">Lorem</div>
                    <div class="text-subtitle2">Subtitle</div>
                  </div>
                </q-img>
                <q-card-section>Un texto</q-card-section>
                <q-card-actions class="row justify-center" >
                  <q-btn flat glossy @click="alerta = true">Más Información</q-btn>
                </q-card-actions>
            </q-card>
        </div>
        <div class="col-4 q-pa-md q-gutter-md">
            <q-card class="my-card" >
                <q-img src="~assets/quasar-logo-vertical.svg">
                  <div class="absolute-bottom">
                    <div class="text-h6">Lorem</div>
                    <div class="text-subtitle2">Subtitle</div>
                  </div>
                </q-img>
                <q-card-section>Un texto</q-card-section>
                <q-card-actions class="row justify-center" >
                  <q-btn flat glossy @click="alerta = true">Más Información</q-btn>
                </q-card-actions> 
            </q-card>
        </div>
    </div>
    <q-dialog v-model="alerta">
        <q-card>
          <q-card-section>
            <div class="text-h6">Más Información</div>
          </q-card-section>

          <q-card-section class="q-pt-none">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum repellendus sit voluptate voluptas eveniet porro. Rerum blanditiis perferendis totam, ea at omnis vel numquam exercitationem aut, natus minima, porro labore.
          </q-card-section>

          <q-card-actions align="right">
            <q-btn flat label="OK" color="primary" v-close-popup />
          </q-card-actions>
        </q-card>
      </q-dialog>
  </q-page>
</template>

<script>
import { ref } from 'vue'
export default {
    setup(){
        return{
            alerta: ref(false)
        }
    }
}
</script>

<style>
</style>