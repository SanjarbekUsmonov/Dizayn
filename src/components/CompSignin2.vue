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

               <q-input outlined  v-model="ph" placeholder="Placeholder" :dense="dense" /> <br>
               <q-input outlined  v-model="ph" placeholder="Placeholder" :dense="dense" /><br>

              <q-btn style="width: 100%;" padding="18px" color="secondary" label="Send Message" />

               <div class="q-mt-lg text-center text-h6 text-weight-regular">
                  Already a member?
                 <a class="a " href="">Singn Up</a>
             </div>
         </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style scoped>
.container{
  width: 100%;
  height: 100vh;
}
.content{
  width: 570px;
  height: 500px;
}
.con{
  width: 500px;
  height: 420px;
}
</style>
