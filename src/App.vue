<template>
  <div id="app">
    <img src="./assets/logo.png">
    {{msg}}
    {{isDone}}
    {{sentence}}
    <!-- {{myFavoriteNumber}} -->
    <router-view/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

@Component({})
export default class App extends Vue {
  data () {
    return {
      like: 999
    }
  }
  msg:string = 'sdfds'
  isDone:boolean = false
  k:number =8
  sentence:string = `hello ,my name is ${this.msg}`
  // myFavoriteNumber:string | number
  alertName ():void {
    // alert('hello')
  }
  mounted () {
    this.alertName()
    // this.myFavoriteNumber = 6
  }
  // 联合类型

  // myFavoriteNumber = 'six'
  // myFavoriteNumber = 6
  // 接口
  // interface person{
  //   name:string;
  //   age:number;
  // }
  onClick ():void {

  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>