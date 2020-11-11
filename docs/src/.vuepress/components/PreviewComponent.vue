<template>
    <router-link :to="productLink" class="preview">
        <i v-if="!isHomePage"></i>
        <img :src="productImage" alt="">
        <h3>{{ productTitle }}</h3>
        <p>{{ productDescription }}</p>
    </router-link>
</template>

<script>
    export default {
        props: [
            'productImage',
            'productLink',
            'productTitle',
            'productDescription'
        ]
    }
</script>

<style lang="scss" scoped>

.preview {
    h3, p {
        margin: 8px 0;
        color: black;
    }
    p {
        opacity: .64;
    }
    &:hover {
        h3, p {
            color: blue;
        }
    }
}


</style>