<template >
  <div>
      <div class="container row justify-center content-center">
        <div class="content bg-grey-1">
           <!-- bosh sarlavha -->
          <div class="contact text-h4 text-weight-bolder">
                Sign In
          </div>
           <!-- bosh sarlavha tugashi-->

           <!-- inputlar boshlanishi -->
             <div class="q-mt-lg">
               <form>
                  <q-input type="email" v-model="email" label="Email" :dense="dense" />
               </form>
             </div>

             <div class="q-mt-xl">
                <form >
                   <q-input type="password" v-model="pwd" label="Password" :dense="dense" />
                </form>
             </div>

           <!-- inputlar tugashi -->
           <div class=" q-mt-xl row  justify-between items-center content-center">
                <q-checkbox  v-model="teal" label="Я не робот" color="teal"/>
              <div class="text-weight-regular">
                  Frgeten Password
              </div>
           </div>

               <div class="q-mt-xl row justify-end">
                  <q-btn style="width: 100%;" padding="18px" color="secondary" label="Send Message" />
               </div>
               <div class="q-mt-lg text-h6 text-weight-regular">
                  Already a member?
                 <a class="a " href="">Singn Up</a>
              </div>

        </div>
      </div>
  </div>
</template>
<script>
import {ref} from "vue"
export default {
  setup () {
     return {
       teal: ref(false),
       email: ref(''),
       pwd: ref(''),
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
.a{
 text-decoration: none;
 color: aqua;
}
</style>
