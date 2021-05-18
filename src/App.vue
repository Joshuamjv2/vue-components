<template>
  <!-- <Greet name='Bruce' heroName='Batman'/>
  <Greet name='Clark' heroName="superman"/>
  <Greet name='Diana' heroName="Wonder woman"/> -->
  <Greet :name="username" :heroName="channel" />



  <Article title="Article Title" :likes="34" :isPublished="true"/>
  <h1>App component username - {{username}}</h1>

</template>

<script>
import Greet from './components/Greet.vue'
import Article from './components/Article.vue'

export default {
  name: 'App',
  components: {
    Greet,
    Article,
  },
  data () {
    return {
      username: 'Joshua Bryant',
      channel: 'Jinja College',
    }
  },
  // provide: {
  //   name: 'Joshua Bryant'
  // }
  provide(){
    return{
      name: this.username
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
