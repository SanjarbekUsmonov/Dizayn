<template>
  <div>
        <!-- bosh sarlavha -->
      <div class="container row justify-center content-center">
        <div class="content bg-grey-1">
          <!-- inputlar boshlanishi -->
            <div class="contact text-h4 text-weight-bolder">
                Contact Us
            </div>
            <div class="q-mt-xl row  justify-between items-start content-start">
                <q-input type="text" class="input-text" v-model="text" label="Name" :dense="dense" />
                 <q-input  type="email" class="input-text" v-model="email" label="Email" :dense="dense" />
            </div>
              <div class="q-mt-xl">
                <q-input  v-model="Subject" label="Subject" :dense="dense" />
              </div>
              <div class="q-mt-xl">
                <q-input  type="textarea"  v-model="textarea" label="Message" :dense="dense" />
              </div>
              <div class="q-mt-xl row justify-end">
                 <q-btn color="secondary" label="Send Message" />
              </div>
              <!-- inputlar tugashi -->
        </div>
      </div>
       <!-- bosh sarlavha tugashi -->
  </div>
</template>
<script>
import { ref } from 'vue'
export default {
    setup () {
    return {
      text: ref(''),
      email: ref(''),
      Subject: ref(''),
      textarea: ref(''),
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
</style>
