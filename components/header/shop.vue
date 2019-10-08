<template>
  <div class="shop-wrapper">
    <div class="shop" @mouseenter="enter" @mouseleave="leave">
      <i class="el-icon-shopping-cart-2"></i>
      购物车
    </div>
    <div class="shop-car" v-if="showcar" @mouseleave="sout" @mouseenter="sover">
      <dl>
        <dt>
          <span class="myCar">我的购物车</span>
          <span class="sum">已加入0门课程</span>
        </dt>
        <dd>购物车里空空如也</dd>
        <dd></dd>
        <!-- <dd class="car-foot">
          <span class>我的订单中心</span>
          <span class>去购物车</span>
        </dd>-->
      </dl>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showcar: false
    }
  },
  methods: {
    enter() {
      this.showcar = true
      console.log(this.showcar)
    },
    leave() {
      let self = this
      self._timer = setTimeout(function() {
        self.showcar = false
      }, 150)
    },
    sover: function() {
      clearTimeout(this._timer)
    },
    sout: function() {
      this.showcar = false
    }
  }
}
</script>
<style lang="css">
.shop-wrapper {
  display: inline-block;
  height: 72px;
  line-height: 72px;
  font-size: 14px;
  position: relative;
}
.shop-wrapper .shop {
  box-sizing: border-box;
  display: inline-block;
  width: 104px;
  height: 36px;
  border: 1px solid #787d82;
  border-radius: 20px;
  padding: 0 18px;
  line-height: 36px;
  margin-right: 20px;
}
.shop-wrapper .shop:hover {
  color: red;
  border: 1px solid red;
}
.shop-wrapper .shop-car {
  /* border: 1px solid #787d82; */
  border-radius: 1px;
  width: 300px;
  height: 300px;
  position: relative;
  right: 100px;
}
.shop-wrapper .shop-car dl dt {
  border-bottom: 1px solid gray;
  margin: 0 15px;
}
.shop-wrapper .shop-car dl dt .myCar {
  font-weight: bold;
}
.shop-wrapper .shop-car dl dt .sum {
  font-size: 10px;
  color: #787d82;
  float: right;
}
.shop-wrapper .shop-car dl dd {
  text-align: center;
}
.shop-wrapper .shop-car dl {
  position: relative;
}
.shop-wrapper .shop-car dl .car-foot {
  border-top: 1px solid gray;
  margin: 0 15px;
  /* position: absolute; */
  bottom: 0;
}
</style>