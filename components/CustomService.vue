<template>
	<div class="CustomService">
		<div class="">
            <div class="service-box floating">
                <nuxt-link to="">
                    <i></i>
                    <span>在线客服</span>
                </nuxt-link>
            </div>
            <div class="top-btn floating">
                <i></i>
            </div>
        </div>
	</div>
</template>

<script>
	export default {
        data(){
            return {
               
            }
        },
		mounted() {
            $(".top-btn").click(function () {
                $('html, body').animate({scrollTop: '0px'}, 500);
            })
		},
        methods: {
        }
	};

</script>

<style lang="scss">
.CustomService {
    position: fixed;
    right: 42px;
    top: 50%;
    transform: translateY(-50%);
    z-index: 99;
    width: 68px;
    .floating {
        border-radius: 10px;
        background-color: #0595a9;
        box-sizing: border-box;
        -webkit-box-shadow: 1px 1px 18px rgba(4, 80, 91, .3); 
        -moz-box-shadow: 1px 1px 18px rgba(4, 80, 91, .3); 
        box-shadow: 1px 1px 18px rgba(4, 80, 91, .3);
        i {
            display: block;
            margin: 0 auto;
            background: url(/images/common/common_icon.png) -33px 0 no-repeat;
        }
    }
    .service-box {
        height: 70px;
        padding: 9px 0 7px;
        i {
            width: 40px;
            height: 36px;
            margin-bottom: 6px;
        }
        span {
            display: block;
            text-align: center;
            color: #fff;
            font-size: 12px;
        }
    }
    .top-btn {
        height: 47px;
        padding: 13px 16px;
        margin-top: 6px;
        cursor: pointer;
        i {
            width: 33px;
            height: 18px;
            background-position: -84px -9px;
        }
    }
}

</style>

