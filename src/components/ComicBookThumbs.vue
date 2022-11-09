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
    width: calc(100% / 6 - 20px);
    margin: 10px;

    img {
        max-height: 180px;

        object-position: top;
        object-fit: cover;
    }

    h4 {
        text-align: start;
        margin-top: .2em;
        font-size: .8rem;
        color: white;
    }
}
</style>