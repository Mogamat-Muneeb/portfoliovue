<template>
<PulseLoader/>
</template>

<script>
import PulseLoader from "vue-spinner/src/PulseLoader.vue"
export default {
    name: "Loader",
    // props: {
    //     color: "",
    // },
    components: {
        PulseLoader,
    }
}
</script>

<style scoped>
    *{
        background: transparent;
        color: #000;
    }

</style>
