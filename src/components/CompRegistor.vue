<template >
  <div>
    <div class="container row justify-center content-center">
        <div class="content bg-grey-1">
          <!-- registor boshlanishi -->
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
           <!-- registor boshlanishi tugashi -->

            <!-- inputlar boshlanishi -->
            <div class="q-mt-lg  row  justify-between items-start content-start">
                <div>
                  <label for="username"><strong>First Name*</strong></label> <br>
                  <input class="first-name" type="text" v-model="Fname" name="Fname">
                </div>
                <div>
                  <label for="username"><strong>Last Name*</strong></label><br>
                  <input class="last-name" type="text" v-model="Lname" name="Lname">
                </div>
            </div>

                  <div class="q-mt-md">
                    <label  for="username"><strong>Username*</strong></label> <br>
                    <input class=" username" type="text" v-model="username" name="username">
                  </div>
                  <div  class="q-mt-md">
                   <label for="email"><strong>Email</strong></label> <br>
                   <input class=" username" type="text" v-model="email" name="email">
                  </div>

             <div class=" row  justify-between items-start content-start">
                  <div class="q-mt-md">
                   <label for="password"><strong>Password</strong></label> <br>
                   <input class="first-name" type="password" v-model="pwd" name="pdw">
                  </div>
                  <div class="q-mt-md">
                   <label for="password"><strong>Confirm Password</strong></label><br>
                   <input class="last-name" type="password" v-model="pwd2" name="pdw">
                 </div>
             </div>
                <!-- inputlar  tugashi -->

              <div class=" q-mt-xl row  justify-between items-center content-center">
                <q-checkbox  v-model="teal" label="Я не робот" color="teal" />
                 <q-btn color="red" icon-right="send" label="Register" />
              </div>
        </div>
    </div>
  </div>
</template>
<script>
import {ref} from "vue"
export default {
    setup () {
    const username = ref('')
    const Fname = ref('')
    const Lname = ref('')
    const email = ref('')
    const pwd = ref('')
    const pwd2 = ref('')

    return {
      teal: ref(false),
      username,
      Fname,
      Lname,
      email,
      pwd,
      pwd2
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
.first-name{
  width: 340px;
  height: 40px;
}
.last-name{
  width: 270px;
  height: 40px;
}
.username{
  width: 100%;
  height: 40px;
}

</style>
