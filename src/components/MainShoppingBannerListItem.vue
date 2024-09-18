<script>
export default {
    data() {
        return {
            
        }
    },
    methods:{
        getImagePath: function(imgPath){
            return new URL(`../assets/img/${imgPath}`, import.meta.url).href;
        }
    },
    props:{
        itemImage: {
            type: String,
            required: true
        },
        itemText: {
            type: String,
            required: true
        },
        itemLink: {
            type: String,
            required: true
        },
    }
}
</script>

<template>
    <article>
        <a :href="itemLink">
            <img :src="getImagePath(itemImage)" alt="">
            <span> {{ itemText }}</span>
        </a>
    </article>
</template>

<style lang="scss" scoped>
article{
    background-color: darkblue;
    
    img{
        height: 60px;    
    }
}
</style>