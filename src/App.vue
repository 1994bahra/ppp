<template>
<div id="app">
  
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
    <div class="navbar-nav">
       <router-link :to="{path: '/', query: {id: 'foo'}}" class="nav-link">
              Home
            </router-link>
       <router-link to="/about" class="nav-link">
              About
            </router-link>
      <router-link to="/education" class="nav-link">
              Education
            </router-link>
       <router-link to="/project" class="nav-link">
              Project
            </router-link>
       <router-link to="/contact" class="nav-link">
              Contact
            </router-link>
    </div>
  </div>
</nav>
<!-- <div id='home'>MY name is Bahra this is my personal website</div> -->
<router-view></router-view>
<!-- <footer><div>bfjkg</div></footer> -->
</div>

</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
 import 'bootstrap/dist/css/bootstrap.css';
 import home from './components/home.vue';
 import { state, setUser } from './app-state'
//  import about from './components/about.vue';
//  import education from './components/education.vue';
//  import project from './components/project.vue';
//  import contact from './components/contact.vue';


export default {
  
  name: 'app',
  components: {
    home
  },
  computed: {
    me: () => state.me
  },
  methods: {
    logout() {
      setUser(null);
      this.$router.push('/');
    }
  }
    
}
</script>

<style>
#app {
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color:black;
  margin-top: 0px;
  background: grey;
  font-size: 1rem;
}
body{
  background: gray;
}


</style>
