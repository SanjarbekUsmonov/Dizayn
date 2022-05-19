<template>
  <div>

      <div class="container row justify-center content-center">
        <div class="content bg-grey-1">
           <!-- bosh sarlavha -->
          <div class="contact text-h4 text-weight-bolder">
                Sign up
          </div>
           <!-- bosh tugashi -->
          <!-- inputlar boshlanishi -->
          <div class="q-mt-xl row  justify-between items-start content-start">
              <q-input type="text" class="input-text" v-model="text" label="Firs Name" :dense="dense" />
               <q-input type="text" class="input-text" v-model="text" label="Last name" :dense="dense" />
          </div>
          <div class="q-mt-xl">
              <q-input type="email" v-model="email" label="Email" :dense="dense" />
          </div>
          <div class="q-mt-xl row  justify-between items-start content-start">
              <q-input  type="password"  class="input-text" v-model="pdw" label="Password" :dense="dense" />
              <q-input type="password" class="input-text" v-model="pdw" label="Confirm Password" :dense="dense" />
          </div>
          <div class="q-mt-xl row justify-end">
                 <q-btn style="width: 100%;" padding="18px" color="secondary" label="Send Message" />
          </div>
          <div class="q-mt-lg text-h6 text-weight-regular">
              Already a member?
              <a class="a " href="">Singn In</a>
          </div>
          <!-- inputlar tugashi -->
         </div>
      </div>


  </div>
</template>
<script>
import { ref } from 'vue'
export default {
    setup () {
    return {
      text: ref(''),
      text : ref(''),
      email: ref(''),
      psw: ref(''),
      pdw: ref(''),
      dense: ref(true)

    }
  }
}
</script>
<style scoped>
.container{
  width: 100%;
  height: 100vh;
}
.content{
  width: 650px;
  height: 550px;
}
.input-text{
  width: 47%;
}
.a{
 text-decoration: none;
 color: aqua;
}
</style>
