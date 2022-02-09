<template>
    <div class="finalfooter">
        <div class="footcontainer">
            <div class="footbar">
                <div class="barcontent">
                    <div>
                        <input type="search">
                        <button>Register</button>
                    </div>
                    <div>
                        <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque aut quaerat magni, eum cupiditate accusamus.
                        </p>
                        <strong>Learn More ></strong>
                    </div>
                </div>
            </div>
            <!-- <div class="contacts" :v-for="(footlink, index) in footinfo">
                <div class="footbox">
                    <h2>{{footinfo.title}}</h2>
                    <ul>
                        <li>{{footinfo.messages}}</li>
                    </ul>
                </div>
                <div class="footbox">
                    <h2>{{footinfo.title}}</h2>
                    <ul>
                        <li>{{footinfo.messages}}</li>
                    </ul>
                </div>
                <div class="footbox">
                    <h2>{{footinfo.title}}</h2>
                    <ul>
                        <li>{{footinfo.messages}}</li>
                    </ul>
                </div>
                <div class="footbox">
                    <h2>{{footinfo.title}}</h2>
                    <ul>
                        <li>{{footinfo.messages}}</li>
                    </ul>
                </div>
            </div> -->

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
    @import '@/style/footerfinal.scss';
</style>