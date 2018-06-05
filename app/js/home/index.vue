<template lang="html">
    <div>
      <Header/>
      <Slider/>
      <Novice/>
      <Fotter/>
    </div>
</template>

<script>
    import Header from '../public/header'
    import Slider from './hsilder'
    import Novice from './novice'
    import Fotter from '../public/footer'
    export default {
        components: {
            Header,
            Slider,
            Novice,
            Fotter
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
