<template lang="html">
    <article>
        <Slider :items="items" :cname="$style.slider"/>
        <section :class="$style.list">
                <div :class="$style.item" v-for="item in enters" :key="item.img">
                    <router-link :to="{name:item.href}"  :class="$style.ddd">
                            <img :src="item.img" :alt="item.title"/>
                            <h4>{{item.title}}</h4>
                    </router-link>
                </div>
        </section>
    </article>
</template>
<script>
import Slider from "../core/slider.vue"
export default {
    components:{
        Slider,
    },
    data() {
			return {
				items: [{
                    href:'home',
                    id:"1",
					src:'//img12.360buyimg.com/jrpmobile/jfs/t24013/135/698019748/49696/3c2fbb63/5b3e03e8N64adfcac.png?width=100%',
				},{
                    href:'home',
                     id:"2",
					src:'//img12.360buyimg.com/jrpmobile/jfs/t23023/109/724585267/42046/46b47d1d/5b3e0417Ne780cc8c.jpg?width=100%'
				},{
                    href:'home',
                     id:"3",
					src:'//img12.360buyimg.com/jrpmobile/jfs/t20812/88/1926208255/43394/af7cfc60/5b3e0437N8b7a1f1b.jpg?width=100%'
				},{
                    href:'home',
                     id:"4",
					src:'//img12.360buyimg.com/jrpmobile/jfs/t23827/131/715725361/51028/9d5a2201/5b3e044cN178bb41b.jpg?width=100%'
				}],
				enters: [{
					href: 'download',
					img: '//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png',
					title: '优惠券',
				}, {
					href: 'download',
					img: '//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png',
					title: '领红包',
				}, {
					href: 'download',
					img: '//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png',
					title: '抢钢镚',
				}, {
					href: 'download',
					img:"//img12.360buyimg.com/jrpmobile/jfs/t12799/50/704102454/5247/19eac80a/5a4f2622Nc4aca701.png",
					title: '领京豆',
				}, {
					href: 'download',
					img: '//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png',
					title: '白条提额',
				}],
			}
		},
}
</script>

<style lang="scss" module>
   @import '../../css/element.scss';
	.slider {
		margin-top: 120px;
		img{
			width:100%;
            display: inline-block;
		}
	}
    .swiper-container-horizontal > .swiper-pagination-bullets{
        bottom: 0px;
    }
	.list {
		@include list(row);
		background: #fff;
        padding-top: 30px;
		justify-content: space-around;
		a {
			text-decoration: none;
		}
		.ddd{
			margin: 20px 10px;
		}
		.item {
			text-align: center;
			img {
				display: inline-block;
				height: 90px;
				width: 90px;
			}
			h4 {
				font-size: 26px;
				margin-top: 12px;
				color: #666;
			}
		}
	}
</style>
