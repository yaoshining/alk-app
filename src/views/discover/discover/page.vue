<template>
    <div>
        <!-- <div class="swiper-container">
            <div class="swiper-wrapper">
                <div class="swiper-slide">
                    <a class="slide-item" href="javascript: void(0)">
                        <img src="http://file.hd.weibo.com/alk/case/jkpr1526471467300.png" alt="">
                    </a>
                </div>
                <div class="swiper-slide">
                    <a class="slide-item" href="javascript: void(0)">
                        <img src="http://file.hd.weibo.com/alk/case/uamo1526471495791.png" alt="">
                    </a>
                </div>
                <div class="swiper-slide">
                    <a class="slide-item" href="javascript: void(0)">
                        <img src="http://file.hd.weibo.com/alk/case/mpyd1526471770704.png" alt="">
                    </a>
                </div>
            </div>
        </div> -->
        <div class="dl-groups">
            <div class="dl-group">
                <dl>
                    <dt>
                        <h3>精选专题</h3>
                    </dt>
                    <dd>
                        <ul class="horizontal-list topic-list">
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    <p>运营小编必看！2018九大蓝V涨</p>
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    <p>运营小编必看！2018九大蓝V涨</p>
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    <p>运营小编必看！2018九大蓝V涨</p>
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    <p>运营小编必看！2018九大蓝V涨</p>
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    <p>运营小编必看！2018九大蓝V涨</p>
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    <p>运营小编必看！2018九大蓝V涨</p>
                                </a>
                            </li>
                        </ul>
                    </dd>
                </dl>
            </div>
            <div class="dl-group">
                <dl>
                    <dt>
                        <h3>行业资讯</h3>
                    </dt>
                    <dd>
                        <ul class="horizontal-list article-list">
                            <li>
                                <a href="javascript: void(0)">
                                    <div>
                                        <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                    </div>
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="javascript: void(0)">
                                    <img src="http://file.hd.weibo.com/alk/content/iizj15292537968921530109919236.png" alt="">
                                </a>
                            </li>
                        </ul>
                    </dd>
                </dl>
            </div>
            <div class="dl-group">
                <dl>
                    <dt>
                        <h3>营销工具</h3>
                    </dt>
                    <dd>
                        
                    </dd>
                </dl>
            </div>
        </div>
    </div>
</template>

<script>
import Swiper from 'swiper';

export default {
    mounted: function() {
        // var mySwiper = new Swiper('.swiper-container', {
            
        // });
    }
}
</script>

<style lang="less" scoped>
.slide-item {
    display: block;
    img {
        width: 100%;
        border-radius: 5px;
    }
}

ul.horizontal-list {
    white-space: nowrap;
    & > li {
        display: inline-block;
        width: 100%;
        margin-right: 5px;
        &:last-child {
            margin-right: 0;
            padding-right: 15px;
        }
        a {
            color: #363636;
        }
        img {
            max-width: 100%;
        }
        p {
            width: 100%;
            white-space: nowrap;
            text-overflow: ellipsis;
            overflow: hidden;
        }
    }
}

.topic-list {
    max-width: 70%;
}

.article-list {
    max-width: 30%;
}

.dl-group {
    padding: 0 0 0 15px;
    margin-bottom: 20px;
    dt {
        border-left: 3px solid #FF5A34;
        padding-left: 5px;
        color: #363636;
        margin: 10px 0;
    }

    dl {
        margin: 0;
    }

    dd {
        margin: 0;
        overflow-x: auto;
        overflow-y: hidden;
        ul {
            list-style: none;
            padding: 0;
        }
    }

}

</style>

<style lang="less">
@import '../../../styles/core.less';
</style>


