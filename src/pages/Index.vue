<template >
  <div>
      <CompRegistor/>
      <CompLogin/>
      <CompContact/>
      <CompSignap/>
      <CompSignin/>
      <CompSignup2/>
      <CompSignin2/>
      <CompRastpdw/>
  </div>
</template>
<script>
import CompRegistor from 'src/components/CompRegistor';
import CompLogin from 'src/components/CompLogin';
import CompContact from 'src/components/CompContact';
import CompSignap from 'src/components/CompSignap';
import CompSignin from '../components/CompSignin';
import CompSignup2 from 'src/components/CompSignup2';
import CompSignin2 from 'src/components/CompSignin2';
import CompRastpdw from '../components/CompRastpdw';
export default {
    components: { CompRegistor, CompLogin, CompContact, CompSignap, CompSignin, CompSignup2, CompSignin2, CompRastpdw }
}
</script>
<style scoped>

</style>
