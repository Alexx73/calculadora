<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App Now bitch"/>
    <div id="row1"> 
          <Boton value="1" 
    color="yellow" 
    :spanX='2'
    :spanY='1'
    />

    <Boton value="2 " 
    :spanX='1'
    :spanY='8'
    />

    <Boton value="3"
      :spanX='1'
      :spanY='7'
    />
    </div>

    



    <!-- <p class="btn">Hello</p> -->
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Boton from '@/components/Boton.vue'



export default {
  name: 'Home',
  
  
  components: {
    HelloWorld,
    // eslint-disable-next-line vue/no-unused-components
    Boton

  }
}
</script>

<style scoped>

.home {
  width: 40%;
  padding: 40px;
  margin-left: auto;
  margin-right: auto;
  border-color: red;
  border-style: solid;

}
</style>
