<template>
    <div id="basicLayout">
        <a-layout style="min-height: 100vh;">
            <a-layout-header class="header">
                <GlobelHeader/>
            </a-layout-header>
            <a-layout-content class="content">
                <!-- <router-view/> -->
            </a-layout-content>
            <a-layout-footer class="footer">
                <a href="http://www.juicew.com" target="_blank">果汁云图库</a>
            </a-layout-footer>
        </a-layout>
    </div>
</template>

<script setup lang="ts">
import GlobelHeader from '@/components/GlobelHeader.vue';


</script>

<style scoped>

#basicLayout .header{
    padding-inline: 20px;
    /* margin-bottom: 16px; */
    color: unset;
    background: white;
}

#basicLayout .content{
    padding: 20px;
    background: linear-gradient(to right, #fefefe, #fff);
    /* margin-bottom: 28px; */
}

#basicLayout .footer{
    background: #efefef;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    text-align: center;
    padding: 16px;

}
</style>


