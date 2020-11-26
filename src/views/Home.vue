<template>
  <div class="about">
    <el-row :gutter="10" class="select-line">
      <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
        <div
          class="grid-content"
          :class="{ active: currentAcitve === 1 }"
          @click="clickTile(1)"
        >
          年会开幕式
        </div>
      </el-col>
      <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
        <div
          class="grid-content"
          :class="{ active: currentAcitve === 2 }"
          @click="clickTile(2)"
        >
          品牌系列榜单
        </div>
      </el-col>
      <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
        <div
          class="grid-content"
          :class="{ active: currentAcitve === 3 }"
          @click="clickTile(3)"
        >
          图片报道
        </div>
      </el-col>
      <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
        <div
          class="grid-content"
          :class="{ active: currentAcitve === 4 }"
          @click="clickTile(4)"
        >
          2020中国茶叶榜
        </div>
      </el-col>
    </el-row>
    <!--资讯-->
    <!--图片展示-->
    <div class="img-box">
      <div class="img-box-title">
        <h2>
          2019中国英德红茶文化节盛大举行
        </h2>
        <span>更多</span>
      </div>

      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
      </el-row>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
      </el-row>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
      </el-row>
    </div>
    <div class="img-box">
      <div class="img-box-title">
        <h2>
          精彩瞬间 - 2020年10月21日
        </h2>
        <span>更多</span>
      </div>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
      </el-row>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <el-image :src="url" :preview-src-list="srcList"> </el-image>
          <p>首长宣布开幕</p>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  data() {
    return {
      currentAcitve: 2,
      url:
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_15.jpg",
      srcList: [
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_15.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_15.jpg",
      ],
    };
  },
  methods: {
    clickTile(num) {
      this.currentAcitve = num;
    },
  },
};
</script>
<style scoped lang="scss">
.img-box {
  background: #fff;
  width: 100%;
  box-sizing: border-box;
  padding: 20px;
  p {
    text-align: left;
  }
  .img-box-title {
    height: 30px;
    line-height: 30px;
    margin-bottom: 20px;
    border: 1px solid #ddd;
    h2 {
      margin: 0;
      padding: 0 0 0 20px;
      float: left;
      border-left: 20px solid #001278;
      font-size: 18px;
    }
    span {
      float: right;
      margin-right: 10px;
      font-size: 14px;
    }
  }
}
.select-line {
  padding-bottom: 40px;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
  line-height: 36px;
  display: block;
  background: #ff9;
  text-align: center;
  border-radius: 100px;
  color: #c00;
  font-size: 16px;
  font-weight: bold;
  margin-bottom: 10px;
  cursor: pointer;
}
</style>
