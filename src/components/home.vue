<template>
  <div id='home'>MY name is Bahra this is my personal website</div>
</template>
<script>
import { state, setUser } from '../app-state.js'
export default {
  data: () => ({
    me: '',
  }),
  methods: {
    home() {
      if (!this.me) return;
      setUser(this.me);
      this.$router.push({path: '/about'})
    }
  }
}
</script>
<style scoped>
#home{
  text-align: center;
  font-size: 2rem;
  margin-top: 10rem;
}
body{
    background-color: brown;
}
</style>
