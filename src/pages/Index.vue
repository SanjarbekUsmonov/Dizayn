<template >
  <div>
      <CompRegistor/>
      <CompLogin/>
      <CompContact/>
  </div>
</template>
<script>
import CompRegistor from 'src/components/CompRegistor';
import CompLogin from 'src/components/CompLogin';
import CompContact from 'src/components/CompContact';
export default {
    components: { CompRegistor, CompLogin,CompContact  }
}
</script>
<style scoped>

</style>
