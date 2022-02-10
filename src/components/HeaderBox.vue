<template>
    <header>
        <div class="headcontainer">
            <div class="logo">
                <img src="@/img/Logo.jpg" alt="">
            </div>
            <div class="navbox" v-for="(link,index) in navList"  v-bind:key="`link-${index}`" >
            <nav class="navbar navbar-expand-lg navbar-light bg-light">
                <div class="collapse navbar-collapse" id="navbarNavDropdown">
                    <ul class="navbar-nav">
                        <li class="nav-item dropdown"> 
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                {{link.navtxt}}
                            </a>
                            <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
                                <a class="dropdown-item" href="#">Action</a>
                                <a class="dropdown-item" href="#">Another action</a>
                                <a class="dropdown-item" href="#">Something else here</a>
                            </div>  
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