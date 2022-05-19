<template>
  <div>
   <div class="container row justify-center content-center">
      <div class="content bg-grey-1 row justify-center content-center">
        <div class="con">
            <div class="contact text-h6 text-weight-bolder">
              Sign up
            </div>
            <div class=" q-mt-lg">
               Complete your registration with
            </div> <br>

              <form >
               <q-input outlined  v-model="psw" type="password" placeholder="Password" :dense="dense" /> <br>
              </form>
               <q-btn style="width: 100%;" padding="18px" color="secondary" label="Send Message" />
         </div>
      </div>
    </div>
  </div>
</template>
<script>
import { ref } from "vue";
export default {
    setup() {
      return{
        psw: ref('')
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
  width: 570px;
  height: 350px;
}
.con{
  width: 500px;
  height: 270px;
}
</style>
