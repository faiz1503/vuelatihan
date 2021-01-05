<template>
  <div id="app">

    <div class="container">
      <div class="row header mb-5 p-3">
        <div class="col-lg-12">
          <h2 class="">Apa yang saya Lakukan Hari Ini</h2>
        </div>
      </div>

      <div class="row content">
        <div class="col-lg-12">
          <div class="pekerjaan-rumah">
            <div class="row">
              <div v-for="tugasSaya in tugas" v-bind:key="tugasSaya.id" class="mb-3 tugas col-lg-12 text-left">
                <ItemTugas1 v-bind:tugasSaya="tugasSaya" />
            </div>
            </div>
          </div>
        </div>
      </div>

    </div>

  </div>
</template>

<script>

import "bootstrap/dist/css/bootstrap.min.css";

import ItemTugas1 from "./components/ItemTugas1.vue";

export default {
  name: "App",
  data: function () {
    return {
      tugas: [
        {
          id: 1,
          namaTugas: "Belajar",
          isDone: false,
        },
        {
          id: 2,
          namaTugas: "Bermain",
          isDone: false,
        },
        {
          id: 3,
          namaTugas: "Tidur",
          isDone: false,
        },
      ],
    };
  },
  components: {
    ItemTugas1
  }
};
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.header {
  background: #1abc9c;
}

.header h2 {
  margin: 0;
}

.tugas .item {
  font-size: 20px;
}

.item-completed {
  color: #1abc9c;
}
</style>
