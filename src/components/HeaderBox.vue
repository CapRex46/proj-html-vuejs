<template>
    <header>
        <div class="headcontainer">
            <div class="logo">
                <img src="@/img/Logo.jpg" alt="">
            </div>
            <div class="navbox" v-for="(link,index) in navList"  v-bind:key="`link-${index}`" >
            <nav>
                <div>
                    <ul>
                        <li> 
                            <a>
                                {{link.navtxt}}
                            </a>

                        </li>
                    </ul>
                </div>
            </nav>


            </div>

        </div>

    </header>
</template>

<script>


export default {
    props: {
        navList: Array,
    }
}
</script>


<style lang="scss" scoped>
@import '@/style/header.scss';
    .headcontainer{
        width: 1400px;
        height: 100px;
        display: flex;
        justify-content: space-between;
        margin: 0 auto;

    }.logo img{
        width: 180px;
        height: 150px;
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        position: relative;
        header{
            width: 100%;
        }
    }

</style>