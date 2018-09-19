<template>
    <section class="container">
        <div>
            <div class="banner">
                <div class="banner-bg">
                    <img src="/images/website/banner.jpg" alt="">
                </div>
                <div class="banner-content content">
                    <h2>专注网站建设9年，精心为您做好网站</h2>
                </div>
            </div>
            <div class="box b1">
                <div class="content">
                    <ul>
                        <li class="li-1">
                            <i></i>
                            <b>三网合一网站建设</b>
                            <span>跨屏浏览自动响应，获得绝佳的访问体验</span>
                            <nuxt-link to="">点击查看</nuxt-link>
                        </li>
                        <li class="li-2">
                            <i></i>
                            <b>小程序</b>
                            <span>体验度极高推广更方便</span>
                            <nuxt-link to="">点击查看</nuxt-link>
                        </li>
                        <li class="li-3">
                            <i></i>
                            <b>微官网</b>
                            <span>快速提升网站排名，获取精准网站流量</span>
                            <nuxt-link to="">点击查看</nuxt-link>
                        </li>
                        <li class="li-4">
                            <i></i>
                            <b>H5</b>
                            <span>一站式H5数字营销平台</span>
                            <nuxt-link to="">点击查看</nuxt-link>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="box b2">
                <div class="content">
                    <ul>
                        <li>
                            <b><i></i>响应式网站（三屏合一）</b>
                            <p>新颖的设计方案,大胆的革新思想,灵活的运用新技术,是在线人的特点,我们只做有灵魂的设计。</p>
                        </li>
                        <li>
                            <b><i></i>做到这四点，才是一个优秀的H5网站</b>
                            <p>三天250,000人次的真实传播量，瞬间让更多人知道你的存在。传播速度快、个性化开发、节省成本、互动性强。</p>
                        </li>
                        <li>
                            <b><i></i>移动圈子四大领域，一个都不能少</b>
                            <p>手机网站、微营销、手机电商、手机应用</p>
                        </li>
                    </ul>
                    <i class="b2-i"></i>
                </div>
            </div>
            <div class="box b3">
                <div class="content">
                    <h4>必达小程序“微”力无边</h4>
                    <h5>从文案架构和网页设计，都是定制策划。每页都精心设计和定制而成</h5>
                    <ul class="clearfix">
                        <li class="li-1">
                            <i></i>
                            <p>微信毫无疑问已是<br/>用户青昧的社交平台</p>
                        </li>
                        <li class="li-2">
                            <i></i>
                            <p>中国手机网名<br/>规模已突破9亿</p>
                        </li>
                        <li class="li-3">
                            <i></i>
                            <p>中国手机网名<br/>规模已突破9亿</p>
                        </li>
                        <li class="li-4">
                            <i></i>
                            <p>四分之一微信用户<br/>每天打开微信的平均<br/>次数出超过30次</p>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="box b4">
                <div class="content">
                    <h4>优秀的项目是这样出来的</h4>
                    <h5>我们一直致力于提供专业的设计解决方案，服务平台涵盖了互联网平台、移动平台，我们用设计为您赢得商机 </h5>
                    <ul class="clearfix">
                        <li class="active">
                            <b class="first-b">1</b>
                            <div class="txt">
                                <b>需求沟通</b>
                                <span>详细了解客户 产品和业务</span>
                            </div>
                        </li>
                        <li>
                            <b class="first-b">2</b>
                            <div class="txt">
                                <b>交互设计</b>
                                <span>根据产品设计 网页功能</span>
                            </div>
                        </li>
                        <li>
                            <b class="first-b">3</b>
                            <div class="txt">
                                <b>视觉创意</b>
                                <span>进行网站页面 美化及创意设计</span>
                            </div>
                        </li>
                        <li>
                            <b class="first-b">4</b>
                            <div class="txt">
                                <b>前端制作</b>
                                <span>制作SEO友好 的html文件</span>
                            </div>
                        </li>
                        <li>
                            <b class="first-b">5</b>
                            <div class="txt">
                                <b>技术开发</b>
                                <span>开发后台功能，测试网站功能</span>
                            </div>
                        </li>
                        <li>
                            <b class="first-b">6</b>
                            <div class="txt">
                                <b>测试反馈</b>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>
.banner {
    height: 320px;
    text-align: center;
    position: relative;
    .banner-bg {
        height: 320px;
        position: absolute;
        left: 0;
        top: 0;
        z-index: -1;
        img {
            width: 100%;
            height: 100%;
        }
    }
    .banner-content {
        padding-top: 128px;
        h2 {
            font-size: 36px;
            color: #fff;
            font-weight: 500;
        }
    }
}

.box {
    text-align: center;
    h4 {
        font-size: 32px;
        color: #333;
    }
    h5 {
        font-size: 14px;
        color: #999;
        margin-top: 40px;
        display: block;
    }
    ul {
        font-size: 0;
        li {
            display: inline-block;
        }
    }
}

.b1 {
    padding: 52px 0 32px;
    ul {
        li {
            width: 228px;
            height: 290px;
            border-radius: 10px;
            background-color: #fff;
            padding: 50px 42px 34px;
            -webkit-box-shadow: 1px 1px 18px rgba(204, 204, 204, .57); 
            -moz-box-shadow: 1px 1px 18px rgba(204, 204, 204, .57); 
            box-shadow: 1px 1px 18px rgba(204, 204, 204, .57);
            margin-left: 70px;
            transition: all .3s;
            i {
                width: 90px;
                height: 57px;
                display: block;
                margin: 0 auto 30px;
                background: url(/images/website/website_icon.png) 0 0 no-repeat;
            }
            b {
                font-size: 18px;
                color: #666;
                display: block;
                margin-bottom: 20px;
            }
            span {
                font-size: 14px;
                color: #999;
                display: block;
                margin-bottom: 20px;
                line-height: 20px;
                height: 40px;
                text-align: justify;
            }
            a {
                width: 100px;
                height: 30px;
                display: inline-block;
                line-height: 30px;
                border-radius: 15px;
                border: 1px solid #33cde5;
                color: #33cde5;
                font-size: 14px;
                transition: all .3s;
            }
            a:hover {
                color: #fff;
                background-color: #33cde5;
            }
        }
        .li-1 {
            margin-left: 0;
        }
        .li-2 {
            i {
                width: 56px;
                background-position-x: -143px;
            }
        }
        .li-3 {
            i {
                width: 70px;
                background-position-x: -262px;
            }
        }
        .li-4 {
            i {
                width: 51px;
                background-position-x: -397px;
            }
        }
        li:hover {
            transform: translateY(-10px);
        }
    }
}

.b2 {
    text-align: left;
    background-color: #f5f5f5;
    padding: 90px 0 70px;
    ul {
        padding-left: 45px;
        box-sizing: border-box;
        li {
            display: block;
            margin-top: 55px;
            width: 325px;
            b {
                font-size: 18px;
                color: #666;
                margin-bottom: 16px;
                display: block;
                i {
                    width: 9px;
                    height: 9px;
                    display: inline-block;
                    background-color: #ffc905;
                    border-radius: 50%;
                    margin-right: 18px;
                    margin-left: -26px;
                    vertical-align: middle;
                }
            }
            p {
                font-size: 14px;
                color: #999;
                line-height: 24px;
            }
        }
        li:first-child {
            margin-top: 0;
        }
    }
    .content {
        position: relative;
        .b2-i {
            width: 546px;
            height: 386px;
            display: inline-block;
            background: url(/images/website/b2_img.png) no-repeat right;
            position: absolute;
            right: 0;
            bottom: 0;
        }
    }
}

.b3 {
    padding: 55px 0 84px;
    ul {
        width: 932px;
        margin: 33px auto 0;
        li {
            float: left;
            width: 173px;
            height: 161px;
            border-radius: 10px;
            padding: 20px 20px 0;
            margin-left: 80px;
            transition: all .3s;
            i {
                width: 75px;
                height: 61px;
                display: block;
                margin: 0 auto 10px;
                background: url(/images/website/website_icon.png) 0 -136px no-repeat;
            }
            p {
                font-size: 14px;
                color: #666;
                line-height: 20px;
            }
        }
        .li-2 {
            i {
                width: 57px;
                background-position-x: -143px;
            }
        }
        .li-3 {
            i {
                width: 57px;
                background-position-x: -262px;
            }
        }
        .li-4 {
            i {
                width: 58px;
                background-position-x: -397px;
            }
        }
        li:hover {
            -webkit-box-shadow: 1px 1px 21px rgba(187, 187, 187, .38); 
            -moz-box-shadow: 1px 1px 21px rgba(187, 187, 187, .38); 
            box-shadow: 1px 1px 21px rgba(187, 187, 187, .38);
        }
        li:first-child {
            margin-left: 0;
        }
    }
}

.b4 {
    padding: 51px 0 101px;
    background-color: #f5f5f5;
    ul {
        margin-top: 77px;
        li {
            width: 212px;
            height: 117px;
            background: url(/images/website/website_icon.png) -243px -267px no-repeat;
            text-align: left;
            margin-left: -22px;
            padding-left: 48px;
            box-sizing: border-box;
            float: left;
            b.first-b {
                font-size: 60px;
                color: #a2a2a2;
                float: left;
                line-height: 117px;
                margin-right: 15px;
            }
            .txt {
                width: 100px;
                display: table-cell;
                height: 117px;
                vertical-align: middle;
                b {
                    font-size: 18px;
                    color: #666;
                    display: block;
                    margin-bottom: 13px;
                }
                span {
                    font-size: 14px;
                    color: #999;
                    line-height: 20px;
                    display: block;
                }
            }
        }
        li:first-child {
            width: 221px;
            background-position-x: 0px;
            padding-left: 37px;
            margin-left: 0;
        }
        li:hover, li.active {
            background-position-y: -454px;
            b.first-b {
                color: #fff;
            }
            .txt {
                b {
                    color: #057081;
                }
                span {
                    color: #fff;
                }
            }
        }
    }
}
</style>