<template>
    <section>
        <div>我是user页，ID应该是可以动态传递的</div>
        <div>{{id}}</div>
        <p>我就是id，值为:{{id}}</p>
    </section>
</template>

<script>
export default {
    data() {
        return {
            id: 123
        }
    },
    components: {},
    mounted() {
        console.log(this.$router);
        console.log(this.$route);
        console.log(this.$route.query);
        console.log(this.$route.params.id);
        this.id = this.$route.params.id;
    },
};
</script>

<style>
</style>
