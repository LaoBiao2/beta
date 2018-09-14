<template>
	<div class="VueHeader">
		<div class="content clearfix">
			<div class="logo">
				<nuxt-link to="/"><img src="/images/common/logo.png" alt=""></nuxt-link>
			</div>
			<ul>
				<!-- <li><nuxt-link to="/">首页</nuxt-link></li>
				<li><nuxt-link to="/1">整合营销</nuxt-link></li>
				<li>
                    <nuxt-link to="/1">新闻营销<i></i></nuxt-link>
                    <div class="sub-menu">
                        <i></i>
                        <nuxt-link to="">网媒营销</nuxt-link>
                        <nuxt-link to="">媒体邀约</nuxt-link>
                        <nuxt-link to="">网站首页</nuxt-link>
                        <nuxt-link to="">客户端发稿</nuxt-link>
                        <nuxt-link to="">报纸发稿</nuxt-link>
                        <nuxt-link to="">软文撰写</nuxt-link>
                    </div>
                </li>
				<li>
                    <nuxt-link to="/1">口碑营销<i></i></nuxt-link>
                    <div class="sub-menu">
                        <i></i>
                        <nuxt-link to="">新闻营销</nuxt-link>
                        <nuxt-link to="">论坛邀约</nuxt-link>
                        <nuxt-link to="">博客营销</nuxt-link>
                        <nuxt-link to="">视频营销</nuxt-link>
                    </div>
                </li>
				<li>
                    <nuxt-link to="/1">移动营销<i></i></nuxt-link>
                    <div class="sub-menu">
                        <i></i>
                        <nuxt-link to="">微博营销</nuxt-link>
                        <nuxt-link to="">微信邀约</nuxt-link>
                        <nuxt-link to="">微博广告</nuxt-link>
                        <nuxt-link to="">陌陌广告</nuxt-link>
                        <nuxt-link to="">直播</nuxt-link>
                        <nuxt-link to="">短视屏</nuxt-link>
                        <nuxt-link to="">H5</nuxt-link>
                        <nuxt-link to="">微信短视频</nuxt-link>
                    </div>
                </li>
				<li>
                    <nuxt-link to="/1">效果广告<i></i></nuxt-link>
                    <div class="sub-menu">
                        <i></i>
                        <nuxt-link to="">微博广告</nuxt-link>
                        <nuxt-link to="">陌陌</nuxt-link>
                        <nuxt-link to="">优酷土豆广告</nuxt-link>
                        <nuxt-link to="">爱奇艺</nuxt-link>
                        <nuxt-link to="">腾讯社交广告</nuxt-link>
                        <nuxt-link to="">微信朋友圈</nuxt-link>
                        <nuxt-link to="">WIFI万能钥匙</nuxt-link>
                    </div>
                </li>
				<li><nuxt-link to="/1">网站优化</nuxt-link></li>
				<li>
                    <nuxt-link to="/1">企业建站<i></i></nuxt-link>
                    <div class="sub-menu">
                        <i></i>
                        <nuxt-link to="">网站建设</nuxt-link>
                        <nuxt-link to="">微官网</nuxt-link>
                        <nuxt-link to="">H5</nuxt-link>
                        <nuxt-link to="">小程序</nuxt-link>
                        <nuxt-link to="">建站案例</nuxt-link>
                    </div>
                </li>
				<li><nuxt-link to="/about">关于我们</nuxt-link></li> -->
                
				<li v-for="(nav, key) in navList" :key="key">
                    <nuxt-link :to="nav.addr" class="first-a">{{nav.title}}<i v-if="nav.sub != ''"></i></nuxt-link>
                </li>
                <div class="sub-menu" v-if="navList[hoverId].sub != ''">
                    <i></i>
                    <nuxt-link :to="sub.addr" v-for="(sub, key2) in navList[hoverId].sub" :key="key2">{{sub.title}}</nuxt-link>
                </div>
			</ul>
		</div>
	</div>
</template>

<script>
import '~/static/animate.css';
	export default {
        data(){
            return {
                navList: [
                    {
                        title: '首页',
                        addr: '/',
                        sub: []
                    }, {
                        title: '整合营销',
                        addr: '/test',
                        sub: []
                    }, {
                        addr: '/test',
                        title: '新闻营销',
                        sub: [
                            { title: '网媒营销', addr: '/test'},
                            { title: '媒体邀约', addr: '/test'},
                            { title: '网站首页', addr: '/test'},
                            { title: '客户端发稿', addr: '/test'},
                            { title: '报纸发稿', addr: '/test'},
                            { title: '软文撰写', addr: '/test'},
                        ]
                    }, {
                        title: '口碑营销',
                        addr: '/test',
                        sub: [
                            { title: '新闻营销', addr: '/test'},
                            { title: '论坛邀约', addr: '/test'},
                            { title: '博客营销', addr: '/test'},
                            { title: '视频营销', addr: '/test'},
                        ]
                    }, {
                        title: '移动营销',
                        addr: '/test',
                        sub: [
                            { title: '微博营销', addr: '/test'},
                            { title: '微信邀约', addr: '/test'},
                            { title: '微博广告', addr: '/test'},
                            { title: '陌陌广告', addr: '/test'},
                            { title: '直播', addr: '/test'},
                            { title: '短视屏', addr: '/test'},
                            { title: 'H5', addr: '/test'},
                            { title: '微信短视频', addr: '/test'},
                        ]
                    }, {
                        title: '效果广告',
                        addr: '/test',
                        sub: [
                            { title: '微博广告', addr: '/test'},
                            { title: '陌陌', addr: '/test'},
                            { title: '优酷土豆广告', addr: '/test'},
                            { title: '爱奇艺', addr: '/test'},
                            { title: '腾讯社交广告', addr: '/test'},
                            { title: '微信朋友圈', addr: '/test'},
                            { title: 'WIFI万能钥匙', addr: '/test'},
                        ]
                    }, {
                        title: '网站优化',
                        addr: '/test',
                        sub: []
                    }, {
                        title: '企业建站',
                        addr: '/website',
                        sub: [
                            { title: '网站建设', addr: '/test'},
                            { title: '微官网', addr: '/test'},
                            { title: 'H5', addr: '/test'},
                            { title: '小程序', addr: '/test'},
                            { title: '建站案例', addr: '/test'},
                        ]
                    }, {
                        title: '关于我们',
                        addr: '/test',
                        sub: []
                    }, 
                ],
                hoverId: 0
            }
        },
		mounted() {
            $(".VueHeader ul li").hover(function () {
                // $(this).find(".sub-menu").addClass("animated fadeInUp");
                // $(this).find(".sub-menu").removeClass("fadeOutDown");
                var liIndex = $(".VueHeader ul li").index(this);
                var liWidth = $(".VueHeader ul li").innerWidth();
                $(".sub-menu").stop(false,true).animate({'left' : (liIndex * liWidth - 18) + 'px'},100);
                this.hoverId = liIndex;
                console.log(this.hoverId);
            },function () {
                // $(this).find(".sub-menu").removeClass("fadeInUp");
                // $(this).find(".sub-menu").addClass("animated fadeOutDown");
            })
		},
        methods: {
        }
	};

</script>

<style lang="scss">
.VueHeader {
	width: 100%;
	height: 76px;
	display: block;
	position: fixed;
	top: 0;
	left: 0;
	z-index: 99;
	background-color: #0a0f2b;
	line-height: 76px;
	.logo {
		width: 190px;
		height: 58px;
		margin: 9px 0;
		float: left;
		img {
			width: 100%;
			height: 100%;
		}
	}
	ul {
		float: right;
		li {
            text-align: center;
			width: 104px;
			display: inline-block;
			line-height: 76px;
			a {
				color: #fff;
                i {
                    width: 9px;
                    height: 6px;
                    display: inline-block;
                    vertical-align: middle;
                    background: url(/images/common/common_icon.png) 0 -24px no-repeat;
                    margin-left: 5px;
                }
			}
            a.nuxt-link-exact-active {
                color: #33cde5;
            }
		}
		li:hover {
			a.first-a {
				color: #33cde5;
                i {
                    background-position-y: -9px;
                }
			}
            // .sub-menu {
            //     max-height: 268px;
            //     i {
            //         display: inline-block;
            //     }
            //     a {
            //         display: block;
            //     }
            // }
        }
        .sub-menu {
            position: relative;
            top: 76px;
            left: -18px;
            width: 135px;
            background-color: #fff;
            padding: 14px 0;
            box-sizing: border-box;
            // max-height: 0px;
            transition: all .3s;
            // opacity: 0;
            i {
                width: 0;
                height: 0;
                border-width: 9px;
                border-style: solid;
                display: inline-block;
                border-color: transparent transparent #fff transparent;
                position: absolute;
                top: -16px;
                left: 50%;
                transform: translateX(-50%);
            }
            a {
                font-size: 16px;
                color: #999;
                line-height: 30px;
                display: block;
                text-align: center;
            }
            a:hover {
                color: #33cde5;
            }

        }
	}
}

@-webkit-keyframes fadeInUp {
  from {
    opacity: 0;
    -webkit-transform: translate3d(0, 20%, 0);
    transform: translate3d(0, 20%, 0);
  }

  to {
    opacity: 1;
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    -webkit-transform: translate3d(0, 20%, 0);
    transform: translate3d(0, 20%, 0);
  }

  to {
    opacity: 1;
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
}

.fadeInUp {
  -webkit-animation-name: fadeInUp;
  animation-name: fadeInUp;
}

@-webkit-keyframes fadeOutDown {
  from {
    opacity: 1;
  }

  to {
    opacity: 0;
    -webkit-transform: translate3d(0, 20%, 0);
    transform: translate3d(0, 20%, 0);
  }
}

@keyframes fadeOutDown {
  from {
    opacity: 1;
  }

  to {
    opacity: 0;
    -webkit-transform: translate3d(0, 20%, 0);
    transform: translate3d(0, 20%, 0);
  }
}

.fadeOutDown {
  -webkit-animation-name: fadeOutDown;
  animation-name: fadeOutDown;
}
</style>

