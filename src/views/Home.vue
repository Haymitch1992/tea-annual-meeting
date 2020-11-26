<template>
  <div class="bj">
    <h1 class="page-title">第十五届中国茶叶经济年会</h1>
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
      <div class="img-box" style="height:400px;">
        <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
          <div class="video-box"></div>
          <dd class="zuzhi">
            <p>指导单位：中华全国供销合作总社</p>
            <br />
            <p>主办单位：中国茶叶流通协会</p>
            <p>广东省农业农村厅</p>
            <p>广东省供销合作联社</p>
            <p>清远市人民政府</p>
            <br />
            <p>承办单位：英德市人民政府、清远市农业农村局</p>
            <br />
            <p>
              协办单位：广东省茶业行业协会等全国各省级茶叶行业组织、英德品牌企业等
            </p>
            <p>执行单位：英德市茶业行业协会</p>
          </dd>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
          <div class="zixun-item">
            <h3>“第十五届中国茶业经济年会暨2019中国英德红茶文化节”盛大举行</h3>
            <p>
              金秋十月丹桂飘香，岭南古驿共襄盛举。10月22日上午，由中国茶叶流通协会、广东省农业农村厅、广东省供销合作联社、清远市人民政府联合主办，英德市人民政府、清远市农业农村局承办，全国各省级茶叶行业组织等单位协办的第十五届中国茶业经济年会暨2019中国英德红茶文化节，在广东省英德市举行了简朴、隆重、热烈的开幕式。<a
                href=""
                >详细>></a
              >
            </p>
          </div>
          <div class="zixun-item">
            <h3>“第十五届中国茶业经济年会暨2019中国英德红茶文化节”盛大举行</h3>
            <p>
              金秋十月丹桂飘香，岭南古驿共襄盛举。10月22日上午，由中国茶叶流通协会、广东省农业农村厅、广东省供销合作联社、清远市人民政府联合主办，英德市人民政府、清远市农业农村局承办，全国各省级茶叶行业组织等单位协办的第十五届中国茶业经济年会暨2019中国英德红茶文化节，在广东省英德市举行了简朴、隆重、热烈的开幕式。<a
                href=""
                >详细>></a
              >
            </p>
          </div>
          <ul class="zixun">
            <li>
              <a
                href="/ctma_news/2019nianhui/news/2019/1028/61300.html"
                target="_blank"
                title="中外茶叶产销对接交流会在英德成功举办"
                >中外茶叶产销对接交流会在英德成功举办</a
              ><!--<span>2019-10-23</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61274"
                target="_blank"
                title="干货满满！中国茶叶质量安全新热点解析与认证可追溯会员专题交流报告会顺利"
                >干货满满！中国茶叶质量安全新热点解析与认证可追溯会员专题交流报告会顺利</a
              ><!--<span>2019-10-23</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61273"
                target="_blank"
                title="会员专题交流报告会——茶业知识产权保护 成功举办"
                >会员专题交流报告会——茶业知识产权保护 成功举办</a
              ><!--<span>2019-10-23</span>-->
            </li>
            <li>
              <a
                href="/ctma_news/2019nianhui/news/2019/1028/61299.html"
                target="_blank"
                title="着眼行业，趋势发布，创新引领，筑梦未来——《2020中国茶叶行业流行趋势》"
                >着眼行业，趋势发布，创新引领，筑梦未来——《2020中国茶叶行业流行趋势》</a
              ><!--<span>2019-10-22</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61270"
                target="_blank"
                title="“第十五届中国茶业经济年会暨2019中国英德红茶文化节”盛大举行"
                >“第十五届中国茶业经济年会暨2019中国英德红茶文化节”盛大举行</a
              ><!--<span>2019-10-22</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61272"
                target="_blank"
                title="精彩不停！第十五届中国茶业经济年会主题报告会成功举办"
                >精彩不停！第十五届中国茶业经济年会主题报告会成功举办</a
              ><!--<span>2019-10-22</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61271"
                target="_blank"
                title="首届国际红茶品牌发展论坛隆重召开"
                >首届国际红茶品牌发展论坛隆重召开</a
              ><!--<span>2019-10-22</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61269"
                target="_blank"
                title="2019年度中国茶叶品牌系列榜单隆重发布"
                >2019年度中国茶叶品牌系列榜单隆重发布</a
              ><!--<span>2019-10-22</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61268"
                target="_blank"
                title="中国茶叶流通协会第六届三次理事会成功召开"
                >中国茶叶流通协会第六届三次理事会成功召开</a
              ><!--<span>2019-10-21</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61267"
                target="_blank"
                title="第一届三次监事会会议顺利召开"
                >第一届三次监事会会议顺利召开</a
              ><!--<span>2019-10-21</span>-->
            </li>
            <li>
              <a
                href="/plus/view.php?aid=61266"
                target="_blank"
                title="英德之夜—CTMA茶客俱乐部·大茶客沙龙活动 华丽绽放"
                >英德之夜—CTMA茶客俱乐部·大茶客沙龙活动 华丽绽放</a
              ><!--<span>2019-10-21</span>-->
            </li>
          </ul>
        </el-col>
      </div>
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
      <pageFooter></pageFooter>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//!非常有用
//?非常有用
// TODO:
import pageFooter from "../components/pageFooter";
export default {
  name: "Home",
  components: {
    pageFooter,
  },
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
  .video-box {
    height: 400px;
  }
  .zuzhi {
    text-align: left;
    border: 1px solid #eee;
    margin: 0;
    p {
      text-align: left;
      font-size: 14px;
      margin: 4px 10px;
    }
  }
  .zixun {
    margin: 0;
    li {
      line-height: 24px;
      font-size: 14px;
      text-align: left;
      a {
        text-decoration: none;
        color: #666;
      }
    }
  }
  .zixun-item {
    padding: 0 10px;
    h3 {
      margin-top: 5px;
      font-size: 26px;
      color: #000;
      font-family: 微软雅黑, 黑体;
      border-left: 4px solid #f00;
      padding-left: 15px;
      border-bottom: 0;
      height: auto;
      text-align: left;
      color: #f00;
    }
    p {
      font-size: 14px;
    }
  }
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
