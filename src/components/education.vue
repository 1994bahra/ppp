<template>

  <div class="row" >
      <div class="container" style="background-image: url('edu.jpg');">
    
</div>
    <div class="col-md-12"><li> I studied at private zhyar high school and graduated in (2012)</li>
</div>
<div class="col-md-12"> <li> studied at salahaddin university college of engineering software<br>
 depertment and graduated in (2016)</li>
</div>
     
  </div>
</template>
<script>
import { state } from '../app-state.js'
//  import 'bootstrap/dist/css/bootstrap.css'; 
export default {
    name: 'education',
  
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
margin-top: 3rem;
font-size: 20px;
text-align: left;
color:skyblue;

}
body{
    background: red;
}
</style>

