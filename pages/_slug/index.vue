<template>
    <section>
        <div>我是_slug路径下面的index</div>
        <p>{{slug}}</p>
    </section>
</template>

<script>
export default {
    data() {
        return {
            slug: ''
        }
    },
    mounted() {
        console.log(this.$route);
        this.slug = this.$route.params.slug;
    },
}
</script>

