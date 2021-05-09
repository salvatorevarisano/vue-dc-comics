<template>
    <div class="comic-thumbnail">
        <div>
            <img :src="comicInfo.thumb" :alt="comicInfo.series">
        </div>
        <div>{{comicInfo.series}}</div>
    </div>
</template>

<script>
export default {
    name: 'Card',

    props: ['comicInfo']
}
</script>

<style lang="scss" scoped>
    .comic-thumbnail {
        font-size: 13px;
        text-transform: uppercase;
        color: #fff; 

        & > div:first-child {
            height: 185px;
            margin-bottom: 20px;
            overflow: hidden;
            img {
                width: 100%;
                object-fit: cover;
            }
        }
    }
</style>
