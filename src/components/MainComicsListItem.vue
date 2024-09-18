<script>
export default {
    data() {
        return {
            
        }
    },
    props: {
        comicUrl: {
            required: true,
            type: String
        },
        comicPrice: {
            required: true,
            type: String
        },
        comicSeries: {
            required: true,
            type: String
        },
        comicType: {
            required: true,
            type: String
        },
    }
}
</script>

<template>
    <li>
        <img :src="comicUrl" :alt="comicSeries">
        <p>
            {{ comicSeries }}
        </p>
    </li>
</template>

<style scoped>
img{
    height: 100px;
}
p{
    font-size: .5rem;
}
</style>