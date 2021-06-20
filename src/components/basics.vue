<!--<template>
  <q-page>
    <div class="row">
      <div class="col-12 text-center bg-dark rounded-borders">
        <h3 class="text-warning">Vue.JS Basico:</h3>
      </div>
      <div class="text-center col-6 q-mt-lg">
        <q-card class="my-card bg-cyan-7 text-white">
          <q-card-section>
            <div class="text-h5">{{ texto }}</div>
            <div class="text-subtitle"></div>
          </q-card-section>

          <q-card-section>
            <q-input
              rounded
              filled
              class="text-subtitle"
              @keyup.esc="BorrarTxt"
              @keyup.enter="alertTxt"
              v-model="texto2"
            >
              <template v-slot:prepend>
                <q-icon name="input" />
              </template>
            </q-input>
            <q-btn @click="BorrarTxt" round class="q-btn--fab q-mt-md bg-dark">
              <q-icon name="backup" />
            </q-btn>
            <div>
              <h4 class="text-subtitle q-mt-md-md">
                {{ texto2 }}
              </h4>
            </div>
          </q-card-section>

          <q-separator dark />

          <q-card-actions>
            <q-btn id="1" flat>Vue Basico</q-btn>
            <q-btn id="2" flat>Vue Medio</q-btn>
          </q-card-actions>
        </q-card>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: "basics",
  data() {
    return {
      llave: "",
      texto: "",
      texto2: "",
    };
  },
  methods: {
    BorrarTxt() {
      this.texto2 = "";
    },

    alertTxt() {
      alert("Datos Obtenidos: " + this.texto2);
    },
  },
};
</script>

<style></style>-->

