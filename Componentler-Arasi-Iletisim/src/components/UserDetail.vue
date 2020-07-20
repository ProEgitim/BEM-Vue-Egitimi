<template>
  <div class="wcol-md-6">
    <h3>Child Component 1</h3>
    <p>Ben User.vue isimli Parent Component'in içerisindeki bir Child componentim</p>
    <p>Kullanıcı Adı: {{name}}</p>
    <p>Kullanıcı Adı Tersten: {{switchName()}}</p>
    <p>Kullanıcı Yaşı: {{age}}</p>
    <button @click="veriyiGonder">Veriyi Parent'a Gönder</button>
  </div>
</template>
<script>
import {eventBus} from '../main';

  export default{
    props: {
      name: {
        type: String,
        default: "Varol Maksutoğlu"
      },
      age: String
    },
    methods:{
      switchName(){
        return this.name.split("").reverse().join("");
      },
      veriyiGonder(){
        this.$emit("data", "VueJS'e Hoşgeldiniz")
      }
    },
    created() {
      eventBus.$on("ageChanged",(age)=>{
        this.age = age;
      })
  }
  }
</script>
<style scoped>
  div {
    background-color: lightcoral;
    padding: 20px;
    border: 1px solid #666;
    display: inline-block;
  }
</style>
