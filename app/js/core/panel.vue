<template>
    <section :class="[panelClass,pName]">
        <h4>-{{title}}-</h4>
        <slot/>
    </section>
    
</template>

<script>
    export default {
        name: "panel.vue",
        props: {
          pName: {
              type: String,
              default: "",
          }
        },
        data () {
            panelClass: 'panel'
        }
    }
</script>

<style lang="scss" scoped>
    @import "../../css/element.scss";
    .panel{
        @include panel;
    }
</style>