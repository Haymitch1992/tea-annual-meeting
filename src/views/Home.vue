<template>
  <div class="bj">
    <!-- <h1 class="page-title">第十五届中国茶叶经济年会</h1> -->
    <div class="about">
      <img
        src="http://www.ctma.com.cn/ctma_news/2020nianhui/style/logo.png"
        alt=""
        class="title-img"
      />
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
            视频报道
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 3 }"
            @click="clickTile(3)"
          >
            精彩瞬间
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 4 }"
            @click="goList()"
          >
            2020中国茶叶榜
          </div>
        </el-col>
      </el-row>
      <!--资讯-->
      <div class="img-box">
        <el-row>
          <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
            <div class="video-box">
              <el-carousel height="380px">
                <el-carousel-item v-for="item in swiperList" :key="item">
                  <a :href="item.target" target="_blank">
                    <img
                      :src="item.imgUrl"
                      style="width:100%;height:380px;"
                      :alt="item.text"
                    />
                    <h2 class="swiper-text">{{ item.text }}</h2>
                  </a>
                </el-carousel-item>
              </el-carousel>
            </div>
            <dd class="zuzhi" style="font-size:13px;">
              <p><b>指导单位：</b></p>
              <p>中华全国供销合作总社</p>
              <p><b>主办单位：</b></p>
              <p>中国茶叶流通协会</p>
              <p>云南省农业农村厅</p>
              <p>云南省供销合作社</p>
              <p>西双版纳傣族自治州人民政府</p>
              <p><b>承办单位：</b></p>
              <p>勐海县人民政府</p>
              <p>西双版纳州农业农村局</p>
              <p>
                <b>承办单位：</b>
              </p>
              <p>云南省茶叶流通协会</p>
              <p>全国各省级茶叶行业组织</p>
            </dd>
          </el-col>
          <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
            <div class="zixun-item">
              <h3>
                第十六届中国茶业经济年会在云南勐海盛大开幕
              </h3>
              <p>
                11月18日，由中华全国供销合作总社指导，中国茶叶流通协会、云南省农业农村厅、云南省供销合作社、西双版纳傣族自治州人民政府主办，勐海县人民政府、西双版纳傣族自治州农业农村局承办，云南省茶叶流通协会等全国各省级茶行业组织协办的“第十六届中国茶业经济年会”在云南省西双版纳州勐海县盛大开幕。
                <a
                  href="http://www.ctma.com.cn/ctma_news/dt/2020/1119/67411.html"
                  target="_blank"
                  >查看详细>></a
                >
              </p>
            </div>
            <div class="zixun-item">
              <h3>
                2020年度茶叶品牌系列榜单隆重发布
              </h3>
              <p>
                11月18日上午，第十六届中国茶业经济年会正式发布了2020年度茶叶行业调查的最终结果。新鲜出炉的行业品牌权威榜单为2020年度茶叶行业调查工作画上完美的句号。
                <a href="/list">查看详细>></a>
              </p>
            </div>
            <ul class="zixun">
              <li v-for="(item, index) in xinwen" :key="index">
                <a :href="item.url" target="_blank" :title="item.text">{{
                  item.text
                }}</a>
              </li>
            </ul>
          </el-col>
        </el-row>
      </div>
      <!--滚动轮播-->
      <div class="img-box">
        <iframe
          width="100%"
          height="170"
          frameborder="0"
          scrolling="no"
          allowtransparency="true"
          id="index_banner"
          src="http://www.ctma.com.cn/ctma_news/2020nianhui/scroll.php"
        ></iframe>
      </div>

      <div class="img-box" id="test2">
        <div class="img-box-title">
          <h2>
            视频报道
          </h2>
        </div>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="24"
            :md="24"
            :lg="24"
            :xl="24"
            @click.native="
              seeViedo(
                'http://go.plvideo.cn/front/video/preview?vid=63d455972fc94152148f2e76528d100f_6'
              )
            "
          >
            <img
              src="https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/v102.jpg"
              alt="第十六届中国茶业经济年会在云南勐海盛大开幕"
              style="width: 100%;height: 675px"
            />
            <p style="color:#666;text-align:center;font-size:12px">
              第十六届中国茶业经济年会在云南勐海盛大开幕
            </p>
          </el-col>
        </el-row>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="24"
            :md="24"
            :lg="24"
            :xl="24"
            @click.native="
              seeViedo(
                'https://dpv.videocc.net/63d455972f/4/63d455972ff6092d29431ffea594d9e4_2.mp4?pid=1606701552234X1153697'
              )
            "
          >
            <img
              src="https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/v106.jpg"
              alt="第十六届中国茶业经济年会在云南勐海盛大开幕"
              style="width: 100%;height: 286px"
            />
            <p style="color:#666;text-align:center;font-size:12px">
              第十六届中国茶业经济年会在云南勐海盛大开幕
            </p>
          </el-col>
        </el-row>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="12"
            :md="12"
            :lg="4"
            :xl="4"
            v-for="item in videoList"
            :key="item.imgUrl"
            @click.native="seeViedo(item.url)"
          >
            <img
              :src="item.img"
              :alt="item.name"
              style="width: 100%;height: 300px"
            />
            <p style="color:#666;text-align:center;font-size:12px">
              嘉宾： {{ item.name }}
            </p>
          </el-col>
        </el-row>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="24"
            :md="24"
            :lg="24"
            :xl="24"
            @click.native="
              seeViedo(
                'http://go.plvideo.cn/front/video/preview?vid=63d455972fcfd90e042925bd982a7293_6'
              )
            "
          >
            <img
              src="http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/v108.jpg"
              alt="第十六届中国茶业经济年会在云南勐海盛大开幕"
              style="width: 100%;height: 675px"
            />
            <p style="color:#666;text-align:center;font-size:12px">
              云南新闻 第五版
            </p>
          </el-col>
        </el-row>
      </div>
      <!-- 视频弹框 -->
      <el-dialog
        title="视频报道"
        :visible.sync="dialogVisible"
        width="70%"
        :before-close="handleClose"
      >
        <iframe
          style="width: 100%;height: 500px"
          frameborder="no"
          allowfullscreen
          mozallowfullscreen
          webkitallowfullscreen
          :src="videoUrl"
        ></iframe>
      </el-dialog>
      <div class="img-box" id="test1">
        <div class="img-box-title">
          <h2>
            “第十六届中国茶业经济年会”盛大举行
          </h2>
          <a
            href="http://www.ctma.com.cn/ctma_news/2020nianhui/news/"
            target="_blank"
            >更多</a
          >
        </div>

        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="12"
            :md="12"
            :lg="12"
            :xl="12"
            v-for="item in imgList1"
            :key="item.imgUrl"
          >
            <a
              :href="
                `http://www.ctma.com.cn/ctma_news/2020nianhui/slide.php?type=${item.type}&id=${item.id}`
              "
              target="_blank"
            >
              <el-image :src="item.imgUrl"> </el-image>
              <p>{{ item.text }}</p></a
            >
          </el-col>
        </el-row>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="12"
            :md="6"
            :lg="6"
            :xl="6"
            v-for="item in imgList2"
            :key="item.imgUrl"
          >
            <a
              :href="
                `http://www.ctma.com.cn/ctma_news/2020nianhui/slide.php?type=${item.type}&id=${item.id}`
              "
              target="_blank"
            >
              <el-image
                :src="item.imgUrl"
                style="width:100%;height:200px !important;"
              >
              </el-image>
              <p>{{ item.text }}</p></a
            >
          </el-col>
        </el-row>
      </div>
      <div class="img-box" id="test3">
        <div class="img-box-title">
          <h2>
            精彩瞬间 - 2020年11月17日
          </h2>
          <a
            href="http://www.ctma.com.cn/ctma_news/2020nianhui/news/"
            target="_blank"
            >更多</a
          >
        </div>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="12"
            :md="6"
            :lg="6"
            :xl="6"
            v-for="item in imgList3"
            :key="item.imgUrl"
          >
            <a
              :href="
                `//www.ctma.com.cn/ctma_news/2020nianhui/slide.php?type=${item.type}&id=${item.id}`
              "
              target="_blank"
            >
              <el-image
                :src="item.imgUrl"
                style="width:100%;height:180px !important;"
              >
              </el-image>
              <p>{{ item.text }}</p></a
            >
          </el-col>
        </el-row>
      </div>
      <div class="img-box">
        <div class="img-box-title">
          <h2>
            精彩瞬间 - 2020年11月18日
          </h2>
          <a
            href="http://www.ctma.com.cn/ctma_news/2020nianhui/news/"
            target="_blank"
            >更多</a
          >
        </div>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="12"
            :md="6"
            :lg="6"
            :xl="6"
            v-for="item in imgList4"
            :key="item.imgUrl"
          >
            <a
              :href="
                `http://www.ctma.com.cn/ctma_news/2020nianhui/slide.php?type=${item.type}&id=${item.id}`
              "
              target="_blank"
            >
              <el-image
                :src="item.imgUrl"
                style="width:100%;height:180px !important;"
              >
              </el-image>
              <p style="height:40px !important;">
                {{ item.text }}
              </p></a
            >
          </el-col>
        </el-row>
      </div>
      <div class="img-box">
        <div class="img-box-title">
          <h2>
            精彩瞬间 - 2020年11月19日
          </h2>
          <a
            href="http://www.ctma.com.cn/ctma_news/2020nianhui/news/"
            target="_blank"
            >更多</a
          >
        </div>
        <el-row :gutter="20">
          <el-col
            :xs="24"
            :sm="12"
            :md="6"
            :lg="6"
            :xl="6"
            v-for="item in imgList5"
            :key="item.imgUrl"
          >
            <a
              :href="
                `http://www.ctma.com.cn/ctma_news/2020nianhui/slide.php?type=${item.type}&id=${item.id}`
              "
              target="_blank"
            >
              <el-image
                :src="item.imgUrl"
                style="width:100%;height:180px !important;"
              >
              </el-image>
              <p>{{ item.text }}</p></a
            >
          </el-col>
        </el-row>
      </div>
      <!--图片展示-->
      <div class="img-box" id="test3">
        <div class="img-box-title">
          <h2>
            辉煌历程
          </h2>
        </div>
        <img
          src="http://www.ctma.com.cn/ctma_news/2020nianhui/style/map.png"
          style="width:100%;display:block;"
          alt=""
        />
      </div>
      <!--位置-->
      <div class="img-box" id="test4">
        <div class="img-box-title">
          <h2>
            年会举办地
          </h2>
        </div>

        <iframe
          src="http://www.ctma.com.cn/map.php?ac=2020nh"
          frameborder="0"
          style="width:100%;height:600px;"
        ></iframe>
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
      videoUrl: "",
      dialogVisible: false,
      // 轮播
      swiperList: [
        {
          text: "第十六届中国茶业经济年会在云南勐海盛大开幕",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111801_11.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1119/67411.html",
        },
        {
          text: "CTMA茶客俱乐部·大茶客沙龙活动圆满落幕",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111701_2.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1119/67405.html",
        },
        {
          text: "第一届四次监事会会议圆满召开",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111702_3.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1119/67406.html",
        },
        {
          text: "中国茶叶流通协会第六届五次理事会成功召开",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111703_1.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1119/67407.html",
        },
        {
          text: "第十六届中国茶业经济年会主题报告会暨产业发展论坛",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111802_1.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1119/67411.html",
        },
        {
          text: "第十六届中国茶业经济年会·经贸洽谈会在勐海成功召开",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111803_23.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1120/67436.html",
        },
        {
          text: "乡村振兴·智慧农业（茶业）发展论坛顺利召开",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111804_2.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1120/67445.html",
        },
        {
          text: "产业热点论坛——普洱茶高峰论坛成功召开",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111901_1.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1120/67437.html",
        },
        {
          text: "振兴中国好茶，公益助农发展”分论坛召开",
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//slide/small/2020111902_10.jpg",
          target: "http://www.ctma.com.cn/ctma_news/dt/2020/1127/67516.html",
        },
      ],
      imgList1: [
        {
          text: "宣布开幕",
          type: 1801,
          id: 14,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/small/2020111801_14.jpg",
        },
        {
          text: "中华全国供销合作总社党组成员、理事会副主任（正部长级）王伟",
          type: 1801,
          id: 11,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/small/2020111801_11.jpg",
        },
      ],
      imgList2: [
        {
          text: "",
          type: 1801,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_1.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 7,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_7.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 8,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_8.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 9,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_9.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 15,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_15.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 16,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_16.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 17,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_17.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 25,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_25.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 28,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_28.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 29,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_29.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 31,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_31.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 32,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_32.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 34,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_34.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 35,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_35.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 44,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_44.jpg",
        },
        {
          text: "",
          type: 1801,
          id: 2,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_2.jpg",
        },
      ],
      imgList3: [
        {
          text: "CTMA茶客俱乐部·大茶客沙龙活动",
          type: 1701,
          id: 2,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111701_2.jpg",
        },
        {
          text: "CTMA茶客俱乐部·大茶客沙龙活动",
          type: 1701,
          id: 4,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111701_4.jpg",
        },
        {
          text: "CTMA茶客俱乐部·大茶客沙龙活动",
          type: 1701,
          id: 8,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111701_8.jpg",
        },
        {
          text: "CTMA茶客俱乐部·大茶客沙龙活动",
          type: 1701,
          id: 9,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111701_9.jpg",
        },
        {
          text: "第一届四次监事会会议",
          type: 1702,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111702_1.jpg",
        },
        {
          text: "第一届四次监事会会议",
          type: 1702,
          id: 2,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111702_2.jpg",
        },
        {
          text: "第一届四次监事会会议",
          type: 1702,
          id: 3,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111702_3.jpg",
        },
        {
          text: "第一届四次监事会会议",
          type: 1702,
          id: 4,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111702_4.jpg",
        },
        {
          text: "第六届五次理事会",
          type: 1703,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111703_1.jpg",
        },
        {
          text: "第六届五次理事会",
          type: 1703,
          id: 37,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111703_37.jpg",
        },
        {
          text: "第六届五次理事会",
          type: 1703,
          id: 65,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111703_65.jpg",
        },
        {
          text: "第六届五次理事会",
          type: 1703,
          id: 66,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111703_66.jpg",
        },
      ],
      imgList4: [
        {
          text: "第十六届中国茶业经济年会盛大开幕",
          type: 1801,
          id: 5,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_5.jpg",
        },
        {
          text: "第十六届中国茶业经济年会盛大开幕",
          type: 1801,
          id: 7,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_7.jpg",
        },
        {
          text: "中华全国供销合作总社党组成员、理事会副主任（正部长级）王伟",
          type: 1801,
          id: 11,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_11.jpg",
        },
        {
          text: "宣布开幕",
          type: 1801,
          id: 14,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_14.jpg",
        },
        {
          text: "中共西双版纳州委副书记、州长罗红江",
          type: 1801,
          id: 8,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_8.jpg",
        },
        {
          text:
            "云南省人民政府原副省长、省政协原副主席、云南省茶叶流通协会创会会长陈勋儒先",
          type: 1801,
          id: 9,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_9.jpg",
        },
        {
          text: "中国茶叶流通协会会长、国家茶叶标准化技术委员会主任委员王庆",
          type: 1801,
          id: 15,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_15.jpg",
        },
        {
          text:
            "云南省人民政府原副省长、省政协原副主席、云南省茶叶流通协会创会会长陈勋儒先",
          type: 1801,
          id: 16,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_16.jpg",
        },
        {
          text: "中华全国供销合作总社党组成员、理事会副主任（正部长级）王伟",
          type: 1801,
          id: 17,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_17.jpg",
        },
        {
          text: "2020年度茶业品牌建设十强县",
          type: 1801,
          id: 27,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_27.jpg",
        },
        {
          text: "十三五’茶业发展十强县",
          type: 1801,
          id: 28,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_28.jpg",
        },
        {
          text: "2020年度茶业创新十强企业",
          type: 1801,
          id: 29,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_29.jpg",
        },
        {
          text: "2020年度茶业社会责任十佳企业",
          type: 1801,
          id: 30,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_30.jpg",
        },
        {
          text: "2020年度茶业百强企业-前十强",
          type: 1801,
          id: 31,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_31.jpg",
        },
        {
          text: "中国制茶大师”（白茶、乌龙茶、花茶类）",
          type: 1801,
          id: 32,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_32.jpg",
        },
        {
          text: "中国茶产业‘十四五’发展规划建议",
          type: 1801,
          id: 33,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_33.jpg",
        },
        {
          text: "会旗交接仪式",
          type: 1801,
          id: 34,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_34.jpg",
        },
        {
          text: "会旗交接仪式",
          type: 1801,
          id: 35,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_35.jpg",
        },
        {
          text: "会旗交接仪式",
          type: 1801,
          id: 37,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_37.jpg",
        },
        {
          text: "品牌发展论坛",
          type: 1801,
          id: 38,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_38.jpg",
        },

        {
          text: "中国茶叶流通协会副会长姚静波",
          type: 1801,
          id: 39,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_39.jpg",
        },
        {
          text: "中国茶叶流通协会副秘书长申卫伟",
          type: 1801,
          id: 40,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_40.jpg",
        },
        {
          text: "第十六届中国茶业经济年会盛大开幕",
          type: 1801,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_1.jpg",
        },
        {
          text: "第十六届中国茶业经济年会盛大开幕",
          type: 1801,
          id: 2,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111801_2.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_1.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 3,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_3.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 4,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_4.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 6,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_6.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 8,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_8.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 9,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_9.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 12,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_12.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 13,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_13.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 14,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_14.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 15,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_15.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 16,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_16.jpg",
        },
        {
          text: "主题报告会暨产业发展论坛",
          type: 1802,
          id: 17,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111802_17.jpg",
        },
        {
          text: "第十六届中国茶业经济年会经贸洽谈会",
          type: 1803,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111803_1.jpg",
        },
        {
          text: "第十六届中国茶业经济年会经贸洽谈会",
          type: 1803,
          id: 3,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111803_3.jpg",
        },
        {
          text: "第十六届中国茶业经济年会经贸洽谈会",
          type: 1803,
          id: 8,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111803_8.jpg",
        },
        {
          text: "第十六届中国茶业经济年会经贸洽谈会",
          type: 1803,
          id: 23,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111803_23.jpg",
        },
        {
          text: "乡村振兴主题论坛",
          type: 1804,
          id: 2,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111804_2.jpg",
        },
        {
          text: "乡村振兴主题论坛",
          type: 1804,
          id: 3,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111804_3.jpg",
        },
        {
          text: "乡村振兴主题论坛",
          type: 1804,
          id: 4,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111804_4.jpg",
        },
        {
          text: "乡村振兴主题论坛",
          type: 1804,
          id: 10,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111804_10.jpg",
        },
      ],
      imgList5: [
        {
          text: "产业热点——普洱茶论坛",
          type: 1901,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111901_1.jpg",
        },
        {
          text: "产业热点——普洱茶论坛",
          type: 1901,
          id: 2,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111901_2.jpg",
        },
        {
          text: "产业热点——普洱茶论坛",
          type: 1901,
          id: 7,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111901_7.jpg",
        },
        {
          text: "产业热点——普洱茶论坛",
          type: 1901,
          id: 11,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111901_11.jpg",
        },
        {
          text: "产业热点——公益助农发展论坛",
          type: 1902,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111902_1.jpg",
        },
        {
          text: "产业热点——公益助农发展论坛",
          type: 1902,
          id: 4,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111902_4.jpg",
        },
        {
          text: "产业热点——公益助农发展论坛",
          type: 1902,
          id: 10,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111902_10.jpg",
        },
        {
          text: "产业热点——公益助农发展论坛",
          type: 1902,
          id: 11,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111902_11.jpg",
        },
        {
          text: "勐海地区茶产业",
          type: 1903,
          id: 1,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111903_1.jpg",
        },
        {
          text: "勐海地区茶产业",
          type: 1903,
          id: 5,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111903_5.jpg",
        },
        {
          text: "勐海地区茶产业",
          type: 1903,
          id: 11,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111903_11.jpg",
        },
        {
          text: "勐海地区茶产业",
          type: 1903,
          id: 18,
          imgUrl:
            "http://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui/slide/thumb/2020111903_18.jpg",
        },
      ],
      videoList: [
        {
          name: "王捷",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v201.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f426d5415b7bc6e5acf985c_6",
        },
        {
          name: "陈慧君",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v202.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f87f79b189e26c303e25048_6",
        },
        {
          name: "陈木艺",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v203.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f86f7338e2532227e493989_6",
        },
        {
          name: "翁荣彬",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v204.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f5d35c4f2f492fb95084cdd_6",
        },
        {
          name: "陈柳滨",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v205.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f37c425f069327769b08e43_6",
        },
        {
          name: "张世影",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v206.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f2d16a368350dd4106e2555_6",
        },

        {
          name: "解方",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v207.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f71b08091cba5fc066d94d2_6",
        },
        {
          name: "傅天龙",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v208.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f21cb13a175768e9e4edfca_6",
        },
        {
          name: "肖文华",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v209.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f290f6dba03327ae27f70a8_6",
        },
        {
          name: "罗振宇",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v210.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972fe928505b74410c6ce07052_6",
        },
        {
          name: "新昌县人民政府副县长",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v211.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f9b53248eda5c4725807ebd_6",
        },
        {
          name: "张志军",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v212.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f9527865eef40f1b9f8e1ab_6",
        },
        {
          name: "林铃顺",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v213.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972fd0cfc059733e5547ef8c0f_6",
        },
        {
          name: "梅宇",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v214.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972fe4eba04670127ab8b7b96e_6",
        },
        {
          name: "阮殿蓉",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v215.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f1acec97d338abc76637eb5_6",
        },
        {
          name: "曹卫",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v216.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f5a9c50f91d1b1808df4d5d_6",
        },
        {
          name: "李晓军",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v217.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972ffb983e25e6f56bd2cf7d04_6",
        },
        {
          name: "林狄昌",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v218.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972faea1f0e181813e2058cde3_6",
        },
        {
          name: "李志圣",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v219.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f47401e314a7aab8234e48d_6",
        },
        {
          name: "王延城",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v220.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f07df14814f0380b17c97b9_6",
        },
        {
          name: "陈世登",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v221.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f3a5977277bde67840ba6e6_6",
        },
        {
          name: "陈兴华",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v222.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f2483778b1215c951b382e1_6",
        },
        {
          name: "陈振林",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v223.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972fcd9685f2046306559cd4b5_6",
        },
        {
          name: "姜竹林",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v224.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972fccb5b9d41ad0d909bbfa81_6",
        },
        {
          name: "马新宏",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v225.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972fe32f7f0a998bfc7602754b_6",
        },
        {
          name: "孙晔",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v226.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f9f85c7599d0ced0fff3dc5_6",
        },
        {
          name: "王启灿",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v227.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f90b9dc53c7e3358fb313c8_6",
        },
        {
          name: "王强",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v228.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f32f602d4ced06baf4b159c_6",
        },
        {
          name: "叶应春",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v229.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f230f3d4e385a85e842837e_6",
        },
        {
          name: "朱富庭",
          img:
            "https://ctmaexpomini.easyking.net.cn/uploads/2020/nianhui//video/cover/s_v230.jpg",
          url:
            "http://go.plvideo.cn/front/video/preview?vid=63d455972f4fd5d6436e3e4e9db2c141_6",
        },
      ],
      xinwen: [
        {
          text: "2020年度茶叶品牌系列榜单隆重发布",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1119/67409.html",
        },
        {
          text: "产业热点论坛——普洱茶高峰论坛成功召开",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1120/67437.html",
        },
        {
          text:
            "“振兴中国好茶”公益扶贫发展分论坛——听中国茶业品牌创新前十品牌小罐茶",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1119/67408.html",
        },
        {
          text:
            "现场达成意向签约13项——第十六届中国茶业经济年会·经贸洽谈会在勐海成功",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1120/67436.html",
        },
        {
          text: "乡村振兴·智慧农业（茶业）发展论坛顺利召开",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1120/67445.html",
        },
        {
          text: "中国茶叶流通协会第六届五次理事会成功召开",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1119/67407.html",
        },
        {
          text: "第一届四次监事会会议圆满召开",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1119/67406.html",
        },
        {
          text: "CTMA茶客俱乐部·大茶客沙龙活动 圆满落幕",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1119/67405.html",
        },
        {
          text: "11月17日，相约此地~",
          url:
            "http://www.ctma.com.cn//ctma_news/2020nianhui/news/2020/1119/67394.html",
        },
        {
          text: "2020中国茶叶集群品牌联盟普洱茶超级单品推荐活动成功举行",
          url: "http://www.ctma.com.cn//ctma_news/dt/2020/1119/67404.html",
        },
        {
          text: "勐海全域旅游指南",
          url:
            "http://www.ctma.com.cn//ctma_news/2020nianhui/news/2020/1119/67403.html",
        },
      ],
      currentAcitve: 2,
      url:
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_01.jpg",
      srcList: [
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_01.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_02.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_03.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_04.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_05.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_06.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_07.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_08.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_09.jpg",
        "http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_10.jpg",
      ],
      timer: "",
    };
  },
  methods: {
    handleClose() {
      this.dialogVisible = false;
    },
    seeViedo(url) {
      this.videoUrl = url;
      this.dialogVisible = true;
    },
    goList() {
      this.$router.push({ path: "/list" });
    },
    clickTile(num) {
      window.location.href = "#test" + num;
      this.currentAcitve = num;
    },
  },
  mounted() {
    // let num = 20;
    // let dom = document.getElementById("cflRollLeft1");
    // let dom2 = document.getElementsByClassName("swiper-box")[0];
    // let _this = this;
    // function start() {
    //   _this.timer = setInterval(() => {
    //     num -= 1;
    //     if (num < -(dom.offsetWidth - dom2.offsetWidth)) {
    //       num = 0;
    //     }
    //     dom.style.left = num + "px";
    //   }, 50);
    // }
    // start();
    // dom.onmousemove = function() {
    //   clearInterval(_this.timer);
    // };
    // dom.onmouseout = function() {
    //   start();
    // };
  },
};
</script>
<style scoped lang="scss">
.swiper-text {
  color: #fff;
  font-weight: normal;
  text-align: center;
  padding: 0;
  background: rgba(0, 0, 0, 0.4);
  width: 100%;
  margin: 0;
  position: absolute;
  top: 0px;
  line-height: 30px;
  font-size: 13px;
  z-index: 100;
}
.title-img {
  display: block;
  width: 100%;
  margin-bottom: 50px;
}
.swiper-box {
  position: relative;
  height: 200px;
}
.img-box {
  overflow: hidden;
  a {
    text-align: left;
    color: #666;
    font-size: 12px;
    text-decoration: none;
  }
  #cflRollLeft1 {
    text-align: left;
    position: absolute;
    left: 0px;
    table {
      padding-right: 10px;
    }
    a {
      text-align: left;
      color: #666;
      font-size: 12px;
      text-decoration: none;
    }
  }
  .video-box {
    height: 380px;
    width: 100%;
    margin: 0 auto 20px;
    background: #ddd;
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
    padding: 10px 10px;
    border-bottom: 1px dashed #ccc;
    margin-bottom: 10px;
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
      font-size: 12px;
      color: #666;
      line-height: 24px;
    }
    a {
      color: #f60;
      padding: 0 10px;
      margin-left: 10px;
      font-size: 12px;
      text-decoration: none;
      float: right;
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
    a {
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
<style>
.el-carousel__button {
  width: 20px !important;
}
</style>
