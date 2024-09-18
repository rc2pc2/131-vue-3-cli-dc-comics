<script>
import MainShoppingBannerListItem from './MainShoppingBannerListItem.vue';

export default {
    components:{
        MainShoppingBannerListItem
    },
    data() {
        return {
            bannerItems: [
                {
                    imageUrl: "buy-comics-digital-comics.png",
                    label: "Digital Comics",
                    link: "#"
                },
                {
                    imageUrl: "buy-comics-merchandise.png",
                    label: "DC Merchandise",
                    link: "#"
                },
                {
                    imageUrl: "buy-comics-subscriptions.png",
                    label: "Subscription",
                    link: "#"
                },
                {
                    imageUrl: "buy-comics-shop-locator.png",
                    label: "Comic Shop Locator",
                    link: "#"
                },
                {
                    imageUrl: "buy-dc-power-visa.svg",
                    label: "DC Power Visa",
                    link: "#"
                },
            ]
        }
    }
}
</script>


<!-- {
    imageUrl: "buy-dc-power-visa.svg",
    label: "DC Power Visa",
    link: "#"
}, -->
<template>
    <h3>
        MainShoppingBannerList
    </h3>
    <section class="banner">

        <MainShoppingBannerListItem v-for="(item, index) in bannerItems" :key="index"
        :itemImage="item.imageUrl"
        :itemText="item.label"
        :itemLink="item.link"
        />
    </section>
</template>

<style scoped>
    section.banner{
        display: flex;
    }
</style>