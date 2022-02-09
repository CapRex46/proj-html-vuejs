<template>
    <div class="campus">
        <div class="infoscampus" v-for="(link,index) in footlink"  v-bind:key="`link-${index}`" >
                <div class="box7">
                    <h2>{{link.title}}</h2>
                    <ul>
                        <li>{{link.msg1}}</li>
                        <li>{{link.msg2}}</li>
                        <li>{{link.msg3}}</li>
                        <li>{{link.msg4}}</li>
                        <li>{{link.msg5}}</li>
                        <li>{{link.msg6}}</li>
                    </ul>                       
            <!-- <div class="box7">
                
            </div>
            <div class="box7">
                
            </div>
            <div class="box7">
                
            </div> -->
        </div>
    </div>
</div>

</template>

<script>
export default {
    props : {
        footlink: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '@/style/footerarray.scss';
</style>






