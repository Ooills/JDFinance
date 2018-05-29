npm <template lang="html">
    <div :class="$style.home">
        <h1>Home</h1>
        <p>Word</p>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" module>
  @import '../../css/reset.scss';
  .home{
    color: red;
    font-size: 80px;
  }
</style>
