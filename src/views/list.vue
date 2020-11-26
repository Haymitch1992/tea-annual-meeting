<template>
  <div class="bj">
    <h1 class="page-title">{{ titleList[currentAcitve - 1] }}</h1>
    <div class="about">
      <!--选项-->
      <el-row :gutter="10" class="select-line">
        <el-col
          :xs="24"
          :sm="12"
          :md="12"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in titleList"
        >
          <div
            class="grid-content"
            :class="{ active: currentAcitve === index + 1 }"
            @click="clickTile(index + 1)"
          >
            {{ item }}
          </div>
        </el-col>
      </el-row>
      <!--百强企业内容-->
      <el-row :gutter="10" v-if="currentAcitve === 1">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top100Data2"
        >
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo" :class="'logo-' + (index + 1)"></div>
            </div>
            <p class="brand-title">{{ item }}</p>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 2">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top100Data"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 3">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju3"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 4">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju4"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 5">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju5"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 6">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju6"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 7">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju7"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 8">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju8"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
    </div>

    <pageFooter></pageFooter>
  </div>
</template>
<script>
import pageFooter from "../components/pageFooter.vue";

export default {
  components: {
    pageFooter,
  },
  data() {
    return {
      currentAcitve: 1,
      titleList: [
        "2020中国茶业百强企业",
        "2020中国茶业百强县",
        "“十三五”茶业发展十强县",
        "2020年度茶业品牌建设十强县",
        "2020年度茶业生态建设十强县",
        "2020年度茶业创新十强企业",
        "2020年度茶业社会责任十佳企业",
        "2020年度茶业新锐十强企业",
      ],
      // 2020年度茶业百强县
      top100Data: [
        "1、贵州省湄潭县",
        "2、福建省安溪县",
        "3、湖南省安化县",
        "4、河南省信阳市浉河区",
        "5、广西壮族自治区横县",
        "6、贵州省凤冈县",
        "7、湖南省长沙县",
        "8、云南省勐海县",
        "9、云南省凤庆县",
        "10、福建省武夷山市",
        "11、四川省雅安市雨城区",
        "12、福建省福鼎市",
        "13、江西省婺源县",
        "14、湖北省英山县",
        "15、浙江省新昌县",
        "16、浙江省松阳县",
        "17、湖北省赤壁市",
        "18、湖北省恩施市",
        "19、湖北省鹤峰县",
        "20、湖南省石门县",
        "21、四川省洪雅县",
        "22、云南省昌宁县",
        "23、湖北省宜昌市夷陵区",
        "24、四川省高县",
        "25、湖北省五峰土家族自治县",
        "26、四川省夹江县",
        "27、湖北省宣恩县",
        "28、福建省福安市",
        "29、广东省英德市",
        "30、湖南省桃源县",
        "31、贵州省石阡县",
        "32、广西壮族自治区昭平县",
        "33、四川省筠连县",
        "34、安徽省歙县",
        "35、陕西省紫阳县",
        "36、云南省临沧市临翔区",
        "37、浙江省武义县",
        "38、山东省日照市岚山区",
        "39、云南省双江拉祜族佤族布朗族傣族自治县",
        "40、安徽省岳西县",

        "41、安徽省休宁县",
        "42、云南省云县",
        "43、河南省光山县",
        "44、贵州省都匀市",
        "45、福建省政和县",
        "46、河南省罗山县",
        "47、四川省邛崃市",
        "48、安徽省祁门县",
        "49、福建省宁德市蕉城区",
        "50、安徽省黄山市徽州区",
        "51、江西省遂川县",
        "52、湖北省宜都市",
        "53、福建省寿宁县",
        "54、安徽省霍山县",
        "55、贵州省黎平县",
        "56、山东省日照市东港区",
        "57、江西省浮梁县",
        "58、湖北省保康县",
        "59、江西省修水县",
        "60、湖北省谷城县",
        "61、安徽省金寨县",
        "62、贵州省正安县",
        "63、云南省永德县",
        "64、河南省商城县",
        "65、浙江省淳安县",
        "66、湖北省咸宁市咸安区",
        "67、河南省新县",
        "68、陕西省泾阳县",
        "69、安徽省黟县",
        "70、湖北省咸丰县",

        "71、安徽省舒城县",
        "72、贵州省余庆县",
        "73、浙江省宁海县",
        "74、云南省景东彝族自治县",
        "75、广西壮族自治区苍梧县",
        "76、浙江省磐安县",
        "77、贵州省金沙县",
        "78、云南省景谷傣族彝族自治县",
        "79、陕西省平利县",
        "80、河南省固始县",
        "81、湖北省长阳土家族自治县",
        "82、江西省铜鼓县",
        "83、广东省大埔县",
        "84、贵州省普安县",
        "85、江苏省常州市金坛区",
        "86、贵州省安顺市西秀区",
        "87、云南省镇康县",
        "88、浙江省景宁畲族自治县",
        "89、湖北省巴东县",
        "90、河南省潢川县",
        "91、福建省光泽县",
        "92、贵州省思南县",
        "93、浙江省龙泉市",
        "94、浙江省天台县",
        "95、湖南省吉首市",
        "96、江西省上犹县",
        "97、广西壮族自治区三江侗族自治县",
        "98、浙江省泰顺县",
        "99、安徽省宁国市",
        "100、广东省紫金县",
      ],
      top100Data2: [
        "1、湖南省茶业集团股份有限公司",
        "2、天福(開曼)控股有限公司",
        "3、浙江华茗园茶业有限公司",
        "4、四川省峨眉山竹叶青茶业有限公司",
        "5、湘丰茶业集团有限公司",
        "6、北京张一元茶叶有限责任公司",
        "7、北京吴裕泰茶业股份有限公司",
        "8、华祥苑茶业股份有限公司",
        "9、萧氏茶业集团有限公司",
        "10、武夷星茶业有限公司",

        "11、湖南华莱生物科技有限公司",
        "12、黄山小罐茶业有限公司",
        "13、福建春伦集团有限公司",
        "14、福建品品香茶业有限公司",
        "15、四川省茶业集团股份有限公司",
        "16、安徽省六安瓜片茶业股份有限公司",
        "17、谢裕大茶叶股份有限公司",
        "18、普洱澜沧古茶股份有限公司",
        "19、湖南省白沙溪茶厂股份有限公司",
        "20、福建新坦洋集团股份有限公司",

        "21、杭州艺福堂茶业有限公司",
        "22、湖北采花茶业有限公司",
        "23、昆明七彩云南庆沣祥茶业股份有限公司",
        "24、羊楼洞茶业股份有限公司",
        "25、云南六大茶山茶业股份有限公司",
        "26、安徽国润茶业有限公司",
        "27、勐海雨林古茶坊茶叶有限责任公司",
        "28、云南双江勐库茶叶有限责任公司",
        "29、广东茶叶进出口有限公司",
        "30、福建省天湖茶业有限公司",

        "31、福建武夷山国家级自然保护区正山茶业有限公司",
        "32、腾冲市高黎贡山生态茶业有限责任公司",
        "33、陕西苍山秦茶集团有限公司",
        "34、河南新林茶业股份有限公司",
        "35、福建省天禧御茶园茶业有限公司",
        "36、勐海陈升茶业有限公司",
        "37、闽榕茶业有限公司",
        "38、信阳市文新茶叶有限责任公司",
        "39、安徽省祁门红茶发展有限公司",
        "40、黄山市猴坑茶业有限公司",

        "41、江西省宁红集团有限公司",
        "42、安徽省抱儿钟秀茶业股份有限公司",
        "43、云南下关沱茶（集团）股份有限公司",
        "44、大不同集团有限公司",
        "45、广西壮族自治区梧州茶厂",
        "46、湖北省茶业集团股份有限公司",
        "47、黄山王光熙松萝茶业股份公司",
        "48、福建鼎白茶业有限公司",
        "49、贵州阳春白雪茶业有限公司",
        "50、益阳茶厂有限公司",
        "51、云南中茶茶业有限公司",
        "52、天方茶业股份有限公司",
        "53、福建康来颜茶业有限公司",
        "54、黄山光明茶业有限公司",
        "55、厦门山国饮艺茶业有限公司",
        "56、恩施州伍家台富硒贡茶有限责任公司",
        "57、黄山紫霞茶业有限公司",
        "58、福建誉达茶业有限公司",
        "59、福州福民茶叶有限公司",
        "60、湖北三品源茶业科技开发有限公司",
        "61、广西梧州茂圣茶业有限公司",
        "62、四川省文君茶业有限公司",
        "63、北京市武夷山老记茶业有限责任公司",
        "64、英德八百秀才茶业有限公司",
        "65、济南博茗茶叶交易中心",
        "66、黄山市新安源有机茶开发有限公司",
        "67、福建瑞达茶业有限公司",
        "68、福建顺茗道茶业有限公司",
        "69、江西省武夷源茶业股份有限公司",
        "70、福建省广福茶业有限责任公司",

        "71、福建省莲峰茶业有限公司",
        "72、海南省农垦五指山茶业集团股份有限公司",
        "73、汉中山花茶业有限公司",
        "74、苏州三万昌茶叶有限公司",
        "75、北京二商京华茶业有限公司",
        "76、江门丽宫国际食品股份有限公司",
        "77、咸阳泾渭茯茶有限公司",
        "78、广东省大埔县西岩茶叶集团有限公司",
        "79、仙居县茶叶实业有限公司",
        "80、贵州湄潭兰馨茶业有限公司",
        "81、广东凯达茶业股份有限公司",
        "82、湖北宜红茶业有限公司",
        "83、湖北汉家刘氏茶业股份有限公司",
        "84、云南农垦集团勐海八角亭茶业有限公司",
        "85、武夷山香江茶业有限公司",
        "86、河南蓝天茶业有限公司",
        "87、浙江诚茂控股集团有限公司",
        "88、广西农垦茶业集团有限公司",
        "89、信阳申林茶业开发有限公司",
        "90、霍山汉唐清茗茶叶有限公司",
        "91、重庆市二圣茶业有限公司",
        "92、罗山县亿峰生态林业开发有限责任公司",
        "93、福建福鼎东南白茶进出口有限公司",
        "94、广西金花茶业有限公司",
        "95、杭州茶厂有限公司",
        "96、四川蒙顶山跃华茶业集团有限公司",
        "97、宁强县千山茶业有限公司",
        "98、河南九华山茶业有限公司",
        "99、福建华香茶业有限公司",
        "100、河南赛山悟道生态茶业科技有限公司",
      ],
      // “十三五”茶业发展十强县
      top10Chaju3: [
        "贵州省湄潭县",
        "福建省安溪县	",
        "湖南省安化县",
        "云南省勐海县",
        "广西壮族自治区横县",
        "河南省信阳市浉河区",
        "福建省福鼎市",
        "浙江省松阳县",
        "安徽省黄山市徽州区",
        "湖北省赤壁市",
      ],
      // 2020年度茶业品牌建设十强县
      top10Chaju4: [
        "广东省英德市",
        "安徽省祁门县	",
        "福建省武夷山市",
        "浙江省新昌县",
        "陕西省泾阳县",
        "贵州省都匀市",
        "云南省双江拉祜族佤族布朗族傣族自治县",
        "江西省浮梁县",
        "四川省筠连县",
        "山东省日照市岚山区",
      ],
      // 2020年度茶业生态建设十强县
      top10Chaju5: [
        "贵州省石阡县",
        "湖南省石门县	",
        "河南省商城县",
        "云南省昌宁县",
        "江西省上犹县",
        "福建省福安市",
        "广西壮族自治区三江侗族自治县",
        "湖北省五峰土家族自治县",
        "安徽省舒城县",
        "四川省邛崃市",
      ],
      //2020年度茶业创新十强企业
      top10Chaju6: [
        "福建品品香茶业有限公司",
        "黄山小罐茶业有限公司	",
        "谢裕大茶叶股份有限公司",
        "杭州艺福堂茶业有限公司",
        "湖南省白沙溪茶厂股份有限公司",
        "安徽省六安瓜片茶业股份有限公司",
        "云南白药天颐茶品有限公司",
        "勐海陈升茶业有限公司",
        "湖北采花茶业有限公司",
        "信阳市文新茶叶有限责任公司",
      ],
      //2020年度茶业社会责任十佳企业
      top10Chaju7: [
        "中国茶叶股份有限公司",
        "八马茶业股份有限公司	",
        "安徽省祁门红茶发展有限公司",
        "福建春伦集团有限公司",
        "四川省茶业集团股份有限公司",
        "云南下关沱茶（集团）股份有限公司",
        "浙江省茶叶集团股份有限公司",
        "广东茶叶进出口有限公司",
        "贵州阳春白雪茶业有限公司",
        "勐海雨林古茶坊茶叶有限责任公司",
      ],
      //2020年度茶业新锐十强企业
      top10Chaju8: [
        "漳州天骏茗风生态农业发展有限公司",
        "湖南省九狮寨高山茶业有限责任公司	",
        "恩施市润邦国际富硒茶业有限公司",
        "广东茗皇茶业有限公司",
        "海南农垦白沙茶业股份有限公司",
        "贵州琦福苑茶业有限公司",
        "云南中吉号茶业有限公司",
        "江苏天目云露茶业有限公司",
        "安徽兰花茶业有限公司",
        "广西顺来茶业有限公司",
      ],
      top10Innovate: [
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
        {
          name: "京华",
          content: "北京二商京华茶业有限公司",
        },
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
.el-col {
  border-radius: 4px;
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
.brand-item {
  .jiang {
    background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/bg_jiang.png)
      no-repeat 50% 50%;
    height: 160px;
    text-align: center;
    width: 245px;
    cursor: pointer;
    border-radius: 6px;
    padding: 0 30px;
    box-sizing: border-box;
    margin: 0 auto;
    vertical-align: middle;
    display: flex;
    /*实现垂直居中*/
    align-items: center;
    /*实现水平居中*/
    justify-content: center;
    flex-wrap: wrap;
    text-align: justify;
    flex-direction: column;
    a {
      font-size: 22px;
      display: block;
      color: #f00;
      font-weight: bold;
      text-shadow: 1px 1px 1px #ff0;
      text-decoration: none;
      text-align: center;
      transition: all 0.5s;
      width: 100%;
    }
  }
  .jiang:hover a {
    font-size: 24px;
  }
  .brand-img {
    width: 245px;
    height: 85px;
    background: #fff;
    border-radius: 6px;
    margin: 0 auto;

    .logo {
      margin: 0 auto;
      width: 125px;
      height: 85px;
      background-image: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg);
    }
    .logo-1 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-2 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px 0px;
    }
    .logo-3 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px 0px;
    }
    .logo-4 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px 0px;
    }
    .logo-5 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px 0px;
    }
    .logo-6 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px 0px;
    }
    .logo-7 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px 0px;
    }
    .logo-8 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px 0px;
    }
    .logo-9 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px 0px;
    }
    .logo-10 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px 0px;
    }
    .logo-11 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -84px;
    }
    .logo-12 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -84px;
    }
    .logo-13 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -84px;
    }
    .logo-14 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -84px;
    }
    .logo-15 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -84px;
    }
    .logo-16 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -84px;
    }
    .logo-17 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -84px;
    }
    .logo-18 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -84px;
    }
    .logo-19 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -84px;
    }
    .logo-20 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -84px;
    }
    .logo-21 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -168px;
    }
    .logo-22 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -168px;
    }
    .logo-23 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -168px;
    }
    .logo-24 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -168px;
    }
    .logo-25 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -168px;
    }
    .logo-26 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -168px;
    }
    .logo-27 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -168px;
    }
    .logo-28 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -168px;
    }
    .logo-29 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -168px;
    }
    .logo-30 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -168px;
    }
    .logo-31 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -252px;
    }
    .logo-32 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -252px;
    }
    .logo-33 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -252px;
    }
    .logo-34 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -252px;
    }
    .logo-35 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -252px;
    }
    .logo-36 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -252px;
    }
    .logo-37 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -252px;
    }
    .logo-38 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -252px;
    }
    .logo-39 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -252px;
    }
    .logo-40 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -252px;
    }
    .logo-41 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -336px;
    }
    .logo-42 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -336px;
    }
    .logo-43 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -336px;
    }
    .logo-44 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -336px;
    }
    .logo-45 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -336px;
    }
    .logo-46 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -336px;
    }
    .logo-47 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -336px;
    }
    .logo-48 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -336px;
    }
    .logo-49 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -336px;
    }
    .logo-50 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -336px;
    }
    .logo-51 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -420px;
    }
    .logo-52 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -420px;
    }
    .logo-53 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -420px;
    }
    .logo-54 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -420px;
    }
    .logo-55 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -420px;
    }
    .logo-56 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -420px;
    }
    .logo-57 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -420px;
    }
    .logo-58 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -420px;
    }
    .logo-59 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -420px;
    }
    .logo-60 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -420px;
    }
    .logo-61 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -504px;
    }
    .logo-62 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -504px;
    }
    .logo-63 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -504px;
    }
    .logo-64 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -504px;
    }
    .logo-65 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -504px;
    }
    .logo-66 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -504px;
    }
    .logo-67 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -504px;
    }
    .logo-68 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -504px;
    }
    .logo-69 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -504px;
    }
    .logo-70 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -504px;
    }
    .logo-71 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -588px;
    }
    .logo-72 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -588px;
    }
    .logo-73 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -588px;
    }
    .logo-74 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -588px;
    }
    .logo-75 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -588px;
    }
    .logo-76 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -588px;
    }
    .logo-77 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -588px;
    }
    .logo-78 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -588px;
    }
    .logo-79 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -588px;
    }
    .logo-80 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -588px;
    }
    .logo-81 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -672px;
    }
    .logo-82 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -672px;
    }
    .logo-83 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -672px;
    }
    .logo-84 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -672px;
    }
    .logo-85 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -672px;
    }
    .logo-86 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -672px;
    }
    .logo-87 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -672px;
    }
    .logo-88 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -672px;
    }
    .logo-89 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -672px;
    }
    .logo-90 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -672px;
    }
    .logo-91 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px -756px;
    }
    .logo-92 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -260px -756px;
    }
    .logo-93 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -474px -756px;
    }
    .logo-94 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -690px -756px;
    }
    .logo-95 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -904px -756px;
    }
    .logo-96 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1114px -756px;
    }
    .logo-97 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1330px -756px;
    }
    .logo-98 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1550px -756px;
    }
    .logo-99 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1760px -756px;
    }
    .logo-100 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -1978px -756px;
    }
  }
  .brand-title {
    color: #ff6;
    font-size: 13px;
    height: 30px;
  }
}
.active {
  background: #c00;
  color: #ff9;
}
</style>
