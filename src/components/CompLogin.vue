<template >
  <div>
      <div class="container  row justify-center content-center">
        <div class="content bg-grey-1">
             <!-- login boshlanishi -->
            <div class="row  justify-start items-center content-center">
              <q-icon size="28px " name="fas fa-user"/>
              <div class="q-ml-md text-h4 text-weight-bolder">
                 Registor
              </div>
              <div class="q-mt-md">
                  Please fill the form below with correct detail to register.
                  if you already have account then Login here.
              </div>
            </div>
           <!-- login tugashi -->
                <!-- inputlar -->
                <div class="q-mt-md">
                    <label  for="username"><strong>Email/Username</strong></label> <br>
                    <input class=" username" type="text" v-model="username" name="username">
                </div>
                <div  class="q-mt-md">
                   <label for="password"><strong>Password</strong></label> <br>
                   <input class=" username" type="password" v-model="paswword" name="password">
                </div>
                <!-- inputlar tugashi -->

                <div class=" q-mt-xl row  justify-between items-center content-center">
                <q-checkbox  v-model="teal" label="Я не робот" color="teal" />
                 <q-btn color="red" icon-right="send" label="Login" />
              </div>

          </div>
      </div>
  </div>
</template>
<script>
import { ref } from "vue";
export default {
    setup() {
      const username = ref('')
      const password = ref('')
      return {
        teal: ref(false),
        username,
        password
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
   height: 450px;
 }
 .username{
  width: 100%;
  height: 40px;
}
</style>
