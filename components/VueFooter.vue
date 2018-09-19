<template>
	<div class="VueFooter">
        <div class="content">
            <div class="footer-top clearfix">
                <div class="logo fl">
                    <img src="/images/common/logo.png" alt="">
                </div>
                <ul class="fr">
                    <li><nuxt-link to="">整合营销</nuxt-link></li>
                    <li><nuxt-link to="">效果广告</nuxt-link></li>
                    <li><nuxt-link to="">新闻营销</nuxt-link></li>
                    <li><nuxt-link to="">报纸发稿</nuxt-link></li>
                    <li><nuxt-link to="">媒体邀约</nuxt-link></li>
                    <li><nuxt-link to="">论坛营销</nuxt-link></li>
                    <li><nuxt-link to="">微博营销</nuxt-link></li>
                    <li><nuxt-link to="">微信营销</nuxt-link></li>
                    <li><nuxt-link to="">口碑营销</nuxt-link></li>
                </ul>
            </div>
            <p>必达广告 - 具有沟通力的整合营销创意</p>
            <div class="p-bottom clearfix">
                <span class="span-copy fl">Copyright © 2013-2018 BETAAD  All Rights Reserved.</span>
                <ul class="fr">
                    <li><span>Links:</span></li>
                    <li><nuxt-link to="/">公众号转让</nuxt-link></li>
                    <li><nuxt-link to="/">宣传片拍摄</nuxt-link></li>
                    <li><nuxt-link to="/">信息流广告</nuxt-link></li>
                    <li><nuxt-link to="/">创意项目</nuxt-link></li>
                    <li><nuxt-link to="/">资源广告</nuxt-link></li>
                </ul>
            </div>
        </div>
	</div>
</template>

<style lang="scss" scoped>
.VueFooter {
	width: 100%;
	height: 175px;
    background-color: #373d41;
    padding: 22px 0 30px;
    box-sizing: border-box;
    .footer-top {
        height: 45px;
        margin-bottom: 30px;
        .logo {
            width: 143px;
            height: 45px;
            img {
                width: 100%;
                height: 100%;
            }
        }
        ul {
            font-size: 0;
            li {
                display: inline-block;
                a {
                    margin-left: 44px;
                    display: block;
                    text-align: right;
                    font-size: 16px;
                    color: #999;
                    line-height: 45px;
                }
            }
        }
    }
    p {
        font-size: 14px;
        color: #999;
    }
	.p-bottom {
        margin-top: 20px;
        font-size: 14px;
        color: #999;
        ul {
            font-size: 0;
            li {
                display: inline-block;
                a {
                    font-size: 14px;
                    color: #999;
                    display: block;
                    margin-left: 20px;
                }
            }
        }
    }
}
</style>

