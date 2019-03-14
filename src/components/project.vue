<template>
<div>
    <h2 id='header'>There are my projects</h2>
  <div class="row" >
      
    <div class="col-md-4"> <img src="p1.png"  width="350" height="200"><br>
    <a href="https://github.com/feb-march-2019-bootcamp/project-1-1994bahra" class="btn btn-info" role="button">Project 1</a>
</div>
<div class="col-md-4"> <img src="p2.png"  width="350" height="200"><br>
    <a href="https://github.com/feb-march-2019-bootcamp/project-2-1994bahra" class="btn btn-info" role="button">Project 2</a>
</div>
<div class="col-md-4"> <img src="p3.png"  width="350" height="200"><br>
    <a href="https://github.com/feb-march-2019-bootcamp/project-3-1994bahra" class="btn btn-info" role="button">Project 3</a>
</div>
<div class="col-md-4"> <img src="p4.png"  width="350" height="200"><br>
    <a href="https://github.com/feb-march-2019-bootcamp/project-4-1994bahra" class="btn btn-info" role="button">Project 4</a>
</div>
<div class="col-md-4"> <img src="p5.png"  width="350" height="200"><br>
    <a href="https://github.com/feb-march-2019-bootcamp/project-5-1994bahra" class="btn btn-info" role="button">Project 5</a>
</div>
<div class="col-md-4"> <img src="p6.png"  width="350" height="200"><br>
    <a href="https://github.com/feb-march-2019-bootcamp/project-6-1994bahra" class="btn btn-info" role="button">Project 6</a>
</div>
  </div>
  </div>
</template>
<script>
import { state } from '../app-state.js'
export default {
    name: 'project',
  
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
margin-top: 1rem;
font-size: 20px;
text-align: left;
color:skyblue;
}
body{
    background: red;
}
#header{
    margin-top: 1rem;
    text-align: center;
    color: blue;
}
</style>

