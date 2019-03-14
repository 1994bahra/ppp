<template>
  <div class="row" >
      
    <div class="col-md-4">
      Name: Bahra Ibrahim Rahman</div>
      <div class="col-md-4">Address: Nusaran, Erbil, Kurdistan Region, Iraq</div>
      <div class="col-md-4">Gender: Female</div>
      <div class="col-md-4">DOB: 14/2/1994</div>
      <div class="col-md-4">Marital Status: Single</div>
      <div class="col-md-4">Nationality: Kurdish</div>
      <div class="col-md-4">Place of Residence: Erbil</div>
      <div class="col-md-4">Mobile: +964 750 8916979</div>
      <div class="col-md-4">Email: bahra.ibrahim9485@gmail.com</div>
    
  </div>
</template>
<script>
import { state } from '../app-state.js'
export default {
    name: 'aboutMe',
  
  methods:{
      created() {
    if (!this.me) {
      this.$router.push('/');
    }
      }
  } 
}
</script>
<style scoped>
.row{
margin-top: 10rem;
font-size: 1rem;
}
</style>

