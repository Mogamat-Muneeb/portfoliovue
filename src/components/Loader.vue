<template>
<PulseLoader color="#00bfff"/>
</template>

<script>
import PulseLoader from "vue-spinner/src/PulseLoader.vue"
export default {
    name: "Loader",
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
