<script>
export default {
    name: "ComicBookThumbs",
    props: {
        imgUrl: String,
        title: String
    }

}
</script>

<template>
    <div class="thumb">
        <img :src="imgUrl" :alt="title">
        <h4>{{ title }}</h4>
    </div>
</template>

<style lang="scss" scoped>
.thumb {
    width: calc(100% / 6 - 10px);
    margin: 5px;

    img {
        max-height: 180px;

        object-position: top;
        object-fit: cover;
    }

    h4 {
        color: white;
        font-size: .8rem;
    }
}
</style>