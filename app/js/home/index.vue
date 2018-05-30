<template lang="html">
    <div>
      <Header/>
    </div>
</template>

<script>
import Header from '../public/header'
export default {
        components: {
            Header
        }
}
</script>

<style lang="scss" module>
  @import '../../css/reset.scss';
  .home{
    color: red;
    font-size: 80px;
  }
</style>
