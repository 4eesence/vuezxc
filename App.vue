<!-- <template>
  <div>
    <input v-model="pervi">
    <input v-model="vtori">
    <button @click="swapText">Поменять</button>
  </div>
</template>

<script>


export default {
  data(){
    return{
      pervi: '',
      vtori: '',
    };
  },


  methods:{
    swapText(){
      let zxc = this.pervi
      this.pervi = this.vtori;
      this.vtori = zxc;
    },
  },

      
  };

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style> -->

<template>
  <div>
    <input v-model="fullimya">
    <button @click="splitRezat">OPABRATZI</button>
    <p>{{ imya }}</p>
    <p>{{ familka }}</p>
    <p>{{ otec }}</p>
  </div>
</template>

<script>


export default {
  data(){
    return{
      fullimya: '',
      imya: '',
      familka: '',
      otec: '',
    };
  },


  methods:{
    splitRezat(){
      let zxc = this.fullimya.split('');
      this.imya = zxc[0];
      this.familka = zxc[1];
      this.otec = zxc[2];
    },

  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
