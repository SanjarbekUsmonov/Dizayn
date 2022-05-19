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
              <!-- inputlar boshlanishi -->
              <form>
                 <q-input outlined type="text" v-model="text" placeholder="Ful Name" :dense="dense" /> <br>
                 <q-input outlined type="email" v-model="email" placeholder="Email" :dense="dense" /><br>
                 <q-input outlined type="password" v-model="pwd1" placeholder="Password" :dense="dense" /><br>
                 <q-input outlined type="password" v-model="pwd2" placeholder="Confirm Password" :dense="dense"/><br>
              </form>
               <!-- inputlar tugashi -->
               <q-checkbox  v-model="teal" label="Я не робот" color="teal"/><br>
               <q-btn style="width: 100%;" padding="18px" color="secondary" label="Send Message" />
              <div class="q-mt-lg text-h6 text-weight-regular">
                  Already a member?
                 <a class="a " href="">Singn Up</a>
              </div>
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
       text: ref(''),
       email: ref(''),
       pwd1: ref(''),
       pwd2: ref(''),
       teal: ref(false),
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
  height: 600px;
}
.con{
  width: 500px;
  height: 530px;
}
</style>
