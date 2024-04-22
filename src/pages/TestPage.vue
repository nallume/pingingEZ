<template>
    <h1>TestPage</h1>
    <div v-for="(t, idx) in state.items" :key="idx">
        {{ t }}
        <MyTest/>
    </div>
</template>
<script>
import MyTest from "@/components/MyTest.vue";
import axios from "axios";
import { reactive } from "vue";
export default {
    name: 'TestPage',
    components: {MyTest}, 
    setup() {
        const state = reactive({
            items:[]
        })
        axios.get("api/test").then((res) => {
            state.items = res.data;
        });
        return {state}
    }
}
</script>
<style scoped>
    
</style>