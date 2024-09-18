<script>
import ComicsList from './MainComicsList.vue';
import ShoppingBannerList from './MainShoppingBannerList.vue';

export default {
    components:{
        ComicsList,
        ShoppingBannerList
    },
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <h2>
        Main
    </h2>
    <ComicsList />
    <ShoppingBannerList />
</template>

<style scoped>
</style>