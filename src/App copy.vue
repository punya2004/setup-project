<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
   <div>
        <!-- <div v-for="data in myJson" :key="data.id">{{data}}</div> -->
         <div class="card comp-card" v-for="data in myJson" :key="data.id">
                                                        <div class="card-body">
                                                            <div class="row align-items-center">
                                                                <div class="col" >
                                                                    <h6 class="m-b-25">{{data.title}}</h6>
                                                                    <h3 class="f-w-700 text-c-blue">6767</h3>
                                                                    <p class="m-b-0">May 23 - June 01 (2017)</p>
                                                                </div>
                                                                <div class="col-auto">
                                                                    <i class="fas fa-eye bg-c-blue"></i>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </div>
    </div>
</template>


<script>
// import HelloWorld from './components/HelloWorld.vue'
import hello from './components/jsons/summary.json'
export default {
  name: 'App',
  components: {
    // HelloWorld
  },
  data(){
              return{
                  myJson: hello.summary,
              }
          }
}
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
