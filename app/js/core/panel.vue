<template>
    <section :class="[panelClass,pName]">
        <h4>-{{title}}-</h4>
        <slot/>
    </section>
    
</template>

<script>
    export default {
        props: {
          pName: {
              type: String,
              default: "",
          }
        },
        data () {
            return {
                panelClass: 'panel',
                title: '新手特权'
            }
        }
    }
</script>

<style lang="scss" scoped>
    @import "../../css/element.scss";
    .panel{
        @include panel;
    }
</style>