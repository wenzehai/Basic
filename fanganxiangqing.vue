<template>
  <div>
    <div class="header">
      <van-nav-bar
              title="方案详情"
              left-arrow
      >
      </van-nav-bar>

    </div>
    <div style="height:46px;"></div>

    <div v-bar="{
    preventParentScroll: true,
    scrollThrottle: 30,
    }">
      <div id="fanganxiangqing" class="main">
        <van-row class="listitem">
          <van-col span="5" class="part1">
            <span class="touzhuIcon iconfont icon-cqssc"></span>
          </van-col>
          <van-col span="13" class="part2">
            <p class="caizhong">重庆时时彩</p>
            <p>投注时间：2018-02-27 16:14:27</p>
            <p>投注订单：TZ0227161427453540</p>
          </van-col>
          <van-col span="6" class="part3">
          </van-col>
        </van-row>

        <van-row class="statusBox">
          <van-col span="8" class="vux-1px-r">
            <p class="des">投注金额</p>
            <p class="money">100.00元</p>
          </van-col>
          <van-col span="8" class="vux-1px-r">
            <p class="des">订单状态</p>
            <p class="money">未中奖</p>
          </van-col>
          <van-col span="8">
            <p class="des">中奖金额</p>
            <p class="money">0.00元</p>
          </van-col>
        </van-row>

        <div class="modelTitle">
          方案内容
        </div>
        <van-row class="fanganlistBox">
          <van-col span="6" class="part5">
            <p class="labelTxt">开奖号码</p>
            <p class="labelTxt">投注内容</p>
            <p class="labelTxt">玩法</p>
            <p class="labelTxt">注数</p>
            <p class="labelTxt">倍数</p>
          </van-col>
          <van-col span="14">
            <p class="contentTxt red">02 11 09 04 06</p>
            <p class="contentTxt">01 03 08 05 07</p>
            <p class="contentTxt">标准,普通玩法,和值</p>
            <p class="contentTxt">21注</p>
            <p class="contentTxt">5倍</p>
          </van-col>
          <van-col span="4">
            <p class="labelTxt">未中奖</p>
          </van-col>
        </van-row>
        <van-row class="fanganlistBox">
          <van-col span="6" class="part5">
            <p class="labelTxt">开奖号码</p>
            <p class="labelTxt">投注内容</p>
            <p class="labelTxt">玩法</p>
            <p class="labelTxt">注数</p>
            <p class="labelTxt">倍数</p>
          </van-col>
          <van-col span="14">
            <p class="contentTxt red">02 11 09 04 06</p>
            <p class="contentTxt">01 03 08 05 07</p>
            <p class="contentTxt">标准,普通玩法,和值</p>
            <p class="contentTxt">21注</p>
            <p class="contentTxt">5倍</p>
          </van-col>
          <van-col span="4">
            <p class="labelTxt">未中奖</p>
          </van-col>
        </van-row>
        <van-row class="fanganlistBox">
          <van-col span="6" class="part5">
            <p class="labelTxt">开奖号码</p>
            <p class="labelTxt">投注内容</p>
            <p class="labelTxt">玩法</p>
            <p class="labelTxt">注数</p>
            <p class="labelTxt">倍数</p>
          </van-col>
          <van-col span="14">
            <p class="contentTxt red">02 11 09 04 06</p>
            <p class="contentTxt">01 03 08 05 07</p>
            <p class="contentTxt">标准,普通玩法,和值</p>
            <p class="contentTxt">21注</p>
            <p class="contentTxt">5倍</p>
          </van-col>
          <van-col span="4">
            <p class="labelTxt">未中奖</p>
          </van-col>
        </van-row>


      </div>
    </div>
    <i-nav></i-nav>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue, Watch } from "vue-property-decorator"
import MarqueeRollUp from "./marquee.vue"
import iNav from "./Nav.vue"

@Component({
  metaInfo() {
    return {
      title: "博乐彩票"
    }
  },
  components: {
    MarqueeRollUp,
    iNav
  },
  data() {
      return {
          active:0,
          tabBars: [
              {
                  id:0,
                  title:'全部'
              },
              {
                  id:1,
                  title:'待开奖'
              },
              {
                  id:2,
                  title:'已中奖'
              }
          ]


      };
  }
})
export default class MyHome extends Vue {
  listData: string[] = ["item1", "item2", "item3"]
  images: any[] = [
    "/static/img/banner/banner1.png",
    "/static/img/banner/banner2.png",
    "/static/img/banner/banner3.png"
  ]


  goUrl(url: string): void {
    this.$router.push(url)
  }
}
</script>

<style scoped>
</style>
