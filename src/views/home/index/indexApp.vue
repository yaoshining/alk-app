<template>
    <div class="page page-index">
        <view-box>
            <x-header slot="header" style="width:100%;position:absolute;left:0;top:0;z-index:100;" title="slot:overwrite-title">
                <div class="overwrite-title-demo" slot="overwrite-title">
                </div>
            </x-header>
            <iframe :src="pageSrc" frameborder="0"></iframe>
            <tabbar slot="bottom"
                    @on-index-change="indexChange">
                <tabbar-item>
                    <img slot="icon" src="./assets/icon_nav_button.png">
                    <span slot="label">首页</span>
                </tabbar-item>
                <tabbar-item show-dot>
                    <img slot="icon" src="@/assets/img/icon_nav_msg.png">
                    <span slot="label">发现</span>
                </tabbar-item>
                <tabbar-item selected link="/component/demo">
                    <img slot="icon" src="./assets/icon_nav_article.png">
                    <span slot="label">案例</span>
                </tabbar-item>
                <tabbar-item badge="2">
                    <img slot="icon" src="./assets/icon_nav_cell.png">
                    <span slot="label">我的</span>
                </tabbar-item>
            </tabbar>
        </view-box>
    </div>
</template>

<script>
import { Tabbar, TabbarItem, Search, ViewBox, XHeader } from 'vux';

export default {
    data: function() {
        return {
            // pageSrc: 'https://www.baidu.com'
            pageSrc: '/views/discover/discover.html'
        }
    },
    components: {
        Search,
        Tabbar,
        ViewBox,
        XHeader,
        TabbarItem
    },
    methods: {
        indexChange: function(index) {
            if(index == 1) {
                this.pageSrc = '/views/discover/discover.html';
            }
        }
    }
}
</script>

<style lang="less" scoped>
.page-index {
    display: flex;
    flex-direction: column;
}

iframe {
    height: 100%;
    width: 100%;
}
</style>


<style lang="less">
@import '../../../styles/core.less';
.page-index {
    #vux_view_box_body {
        padding: 46px 0 55px 0;
    }
}
</style>
