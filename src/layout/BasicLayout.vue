<template>
    <div id="basicLayout">
        <a-layout style="min-height: 100vh;">
            <a-layout-header class="header">
                <GlobelHeader/>
            </a-layout-header>
            <a-layout>
                <GlobelSider class="sider" />
                <a-layout-content class="content">
                    <router-view />
                </a-layout-content>
            </a-layout>

            <a-layout-footer class="footer">
                <a href="http://www.juicew.com" target="_blank">果汁云图库</a>
            </a-layout-footer>
        </a-layout>
    </div>
</template>

<script setup lang="ts">
import GlobelHeader from '@/components/GlobelHeader.vue';
import GlobelSider from '@/components/GlobelSider.vue';

</script>

<style scoped>

#basicLayout .header{
    padding-inline: 20px;
    /* margin-bottom: 16px; */
    color: unset;
    background: white;
    margin-bottom: 1px;
}

#basicLayout .content{
    padding: 28px;
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

#basicLayout .sider {
  background: #fff;
  padding-top: 20px;
  border-right: 0.5px solid #eee;
}

#basicLayout :deep(.ant-menu-root) {
  border-bottom: none !important;
  border-inline-end: none !important;
}

</style>


