<template>
    <div class="imgfoot">
        <img src="@/img/course-1-1.jpg" alt="">
        <img src="@/img/course-1-2.jpg" alt="">
        <img src="@/img/course-1-3.jpg" alt="">
        <img src="@/img/news-3-2.jpg" alt="">
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    .imgfoot{
        width: 100%;
        display: flex;
        margin-top: 80px;
        img {
            width: calc(100% / 4);
            height: 300px;
        }
    }
</style>