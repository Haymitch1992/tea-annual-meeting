<template>
  <div class="bj">
    <h1 class="page-title">2020中国茶叶百强企业</h1>
    <div class="about">
      <!--选项-->
      <el-row :gutter="10" class="select-line">
        <el-col :xs="24" :sm="12" :md="12" :lg="4" :xl="4">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 1 }"
            @click="clickTile(1)"
          >
            2019中国茶业百强县
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="5" :xl="5">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 2 }"
            @click="clickTile(2)"
          >
            2019中国茶业百强企业
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="5" :xl="5">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 3 }"
            @click="clickTile(3)"
          >
            2019中国茶旅融合十强示范县
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="5" :xl="5">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 4 }"
            @click="clickTile(4)"
          >
            2019中国十大生态产茶县
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="5" :xl="5">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 5 }"
            @click="clickTile(5)"
          >
            2019中国茶业最具创新力品牌
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 6 }"
            @click="clickTile(6)"
          >
            2019中国茶业最受消费者认可品牌
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 7 }"
            @click="clickTile(7)"
          >
            2019中国茶业最佳市场运行品牌
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 8 }"
            @click="clickTile(8)"
          >
            2019中国茶业最具传播力品牌
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6">
          <div
            class="grid-content"
            :class="{ active: currentAcitve === 9 }"
            @click="clickTile(9)"
          >
            2019中国茶业年度特别贡献企业
          </div>
        </el-col>
      </el-row>
      <!--百强企业内容-->
      <el-row :gutter="10" v-if="currentAcitve === 1">
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">1、湖南省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-2"></div>
            </div>
            <p class="brand-title">2、天福(開曼)控股有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-3"></div>
            </div>
            <p class="brand-title">3、四川省峨眉山竹叶青茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-4"></div>
            </div>
            <p class="brand-title">4、浙江华茗园茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-5"></div>
            </div>
            <p class="brand-title">5、湘丰茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-6"></div>
            </div>
            <p class="brand-title">6、北京张一元茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-7"></div>
            </div>
            <p class="brand-title">7、北京吴裕泰茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-8"></div>
            </div>
            <p class="brand-title">8、黄山小罐茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-9"></div>
            </div>
            <p class="brand-title">9、萧氏茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-10"></div>
            </div>
            <p class="brand-title">10、武夷星茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-11"></div>
            </div>
            <p class="brand-title">11、福建品品香茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">12、福建春伦集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">13、谢裕大茶叶股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">14、云南下关沱茶（集团）股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">15、勐海雨林古茶坊茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">16、湖南省白沙溪茶厂股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">17、四川省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">18、福建省天湖茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">19、益阳茶厂有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">20、安徽省六安瓜片茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">1、湖南省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-2"></div>
            </div>
            <p class="brand-title">2、天福(開曼)控股有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-3"></div>
            </div>
            <p class="brand-title">3、四川省峨眉山竹叶青茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-4"></div>
            </div>
            <p class="brand-title">4、浙江华茗园茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-5"></div>
            </div>
            <p class="brand-title">5、湘丰茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-6"></div>
            </div>
            <p class="brand-title">6、北京张一元茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-7"></div>
            </div>
            <p class="brand-title">7、北京吴裕泰茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-8"></div>
            </div>
            <p class="brand-title">8、黄山小罐茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-9"></div>
            </div>
            <p class="brand-title">9、萧氏茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-10"></div>
            </div>
            <p class="brand-title">10、武夷星茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-11"></div>
            </div>
            <p class="brand-title">11、福建品品香茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">12、福建春伦集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">13、谢裕大茶叶股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">14、云南下关沱茶（集团）股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">15、勐海雨林古茶坊茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">16、湖南省白沙溪茶厂股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">17、四川省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">18、福建省天湖茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">19、益阳茶厂有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">20、安徽省六安瓜片茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">1、湖南省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-2"></div>
            </div>
            <p class="brand-title">2、天福(開曼)控股有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-3"></div>
            </div>
            <p class="brand-title">3、四川省峨眉山竹叶青茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-4"></div>
            </div>
            <p class="brand-title">4、浙江华茗园茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-5"></div>
            </div>
            <p class="brand-title">5、湘丰茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-6"></div>
            </div>
            <p class="brand-title">6、北京张一元茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-7"></div>
            </div>
            <p class="brand-title">7、北京吴裕泰茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-8"></div>
            </div>
            <p class="brand-title">8、黄山小罐茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-9"></div>
            </div>
            <p class="brand-title">9、萧氏茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-10"></div>
            </div>
            <p class="brand-title">10、武夷星茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-11"></div>
            </div>
            <p class="brand-title">11、福建品品香茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">12、福建春伦集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">13、谢裕大茶叶股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">14、云南下关沱茶（集团）股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">15、勐海雨林古茶坊茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">16、湖南省白沙溪茶厂股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">17、四川省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">18、福建省天湖茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">19、益阳茶厂有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">20、安徽省六安瓜片茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">1、湖南省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-2"></div>
            </div>
            <p class="brand-title">2、天福(開曼)控股有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-3"></div>
            </div>
            <p class="brand-title">3、四川省峨眉山竹叶青茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-4"></div>
            </div>
            <p class="brand-title">4、浙江华茗园茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-5"></div>
            </div>
            <p class="brand-title">5、湘丰茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-6"></div>
            </div>
            <p class="brand-title">6、北京张一元茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-7"></div>
            </div>
            <p class="brand-title">7、北京吴裕泰茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-8"></div>
            </div>
            <p class="brand-title">8、黄山小罐茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-9"></div>
            </div>
            <p class="brand-title">9、萧氏茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-10"></div>
            </div>
            <p class="brand-title">10、武夷星茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-11"></div>
            </div>
            <p class="brand-title">11、福建品品香茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">12、福建春伦集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">13、谢裕大茶叶股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">14、云南下关沱茶（集团）股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">15、勐海雨林古茶坊茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">16、湖南省白沙溪茶厂股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">17、四川省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">18、福建省天湖茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">19、益阳茶厂有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">20、安徽省六安瓜片茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">1、湖南省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-2"></div>
            </div>
            <p class="brand-title">2、天福(開曼)控股有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-3"></div>
            </div>
            <p class="brand-title">3、四川省峨眉山竹叶青茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-4"></div>
            </div>
            <p class="brand-title">4、浙江华茗园茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-5"></div>
            </div>
            <p class="brand-title">5、湘丰茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-6"></div>
            </div>
            <p class="brand-title">6、北京张一元茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-7"></div>
            </div>
            <p class="brand-title">7、北京吴裕泰茶业股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-8"></div>
            </div>
            <p class="brand-title">8、黄山小罐茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-9"></div>
            </div>
            <p class="brand-title">9、萧氏茶业集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-10"></div>
            </div>
            <p class="brand-title">10、武夷星茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-11"></div>
            </div>
            <p class="brand-title">11、福建品品香茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">12、福建春伦集团有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">13、谢裕大茶叶股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">14、云南下关沱茶（集团）股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">15、勐海雨林古茶坊茶叶有限责任公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">16、湖南省白沙溪茶厂股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">17、四川省茶业集团股份有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">18、福建省天湖茶业有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">19、益阳茶厂有限公司</p>
          </div>
        </el-col>
        <el-col :xs="12" :sm="6" :md="6" :lg="6" :xl="6">
          <div class="brand-item">
            <div class="brand-img">
              <div class="logo logo-1"></div>
            </div>
            <p class="brand-title">20、安徽省六安瓜片茶业股份有限公司</p>
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
      <!--十大茶具-->
      <el-row :gutter="10" v-if="currentAcitve === 3">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10County"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <!--十大茶具-->
      <el-row :gutter="10" v-if="currentAcitve === 4">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Chaju"
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
          v-for="(item, index) in top10Innovate"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item.name }}</a>
              <a href="javascript:;" style="font-size:16px;">{{
                item.content
              }}</a>
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
          v-for="(item, index) in top10Innovate"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item.name }}</a>
              <a href="javascript:;" style="font-size:16px;">{{
                item.content
              }}</a>
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
          v-for="(item, index) in top10Innovate"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item.name }}</a>
              <a href="javascript:;" style="font-size:16px;">{{
                item.content
              }}</a>
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
          v-for="(item, index) in top10Innovate"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item.name }}</a>
              <a href="javascript:;" style="font-size:16px;">{{
                item.content
              }}</a>
            </div>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" v-if="currentAcitve === 9">
        <el-col
          :xs="12"
          :sm="6"
          :md="6"
          :lg="6"
          :xl="6"
          :key="index"
          v-for="(item, index) in top10Innovate"
        >
          <div class="brand-item">
            <div class="jiang">
              <a href="javascript:;">{{ item.name }}</a>
              <a href="javascript:;" style="font-size:16px;">{{
                item.content
              }}</a>
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
      currentAcitve: 2,
      top100Data: [
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
        "1、湖南省益阳市安化县",
        "2、贵州省遵义市湄潭县",
        "3、福建省泉州市安溪县",
        "4、广西壮族自治区南宁市横县",
        "5、河南省信阳市浉河区",
      ],
      top10County: [
        "福建南平武夷山市",
        "浙江绍兴新昌县	",
        "贵州遵义湄潭县",
        "广东清远英德市",
        "安徽黄山徽州区",
        "广西南宁横县",
        "河南信阳罗山县",
        "湖北宜昌五峰土家族自治县",
        "江西景德镇浮梁县",
        "四川宜宾高县",
      ],
      top10Chaju: [
        "福建南平武夷山市",
        "浙江绍兴新昌县	",
        "贵州遵义湄潭县",
        "广东清远英德市",
        "安徽黄山徽州区",
        "广西南宁横县",
        "河南信阳罗山县",
        "湖北宜昌五峰土家族自治县",
        "江西景德镇浮梁县",
        "四川宜宾高县",
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
    height: 150px;
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
    }
    .logo-1 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-2 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-3 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-4 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-5 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-6 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-7 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-8 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-9 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-10 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-11 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
    .logo-12 {
      background: url(http://www.ctma.com.cn/ctma_news/2019nianhui/baiqiang/2.jpg)
        no-repeat -44px 0px;
    }
  }
  .brand-title {
    color: #ff6;
    font-size: 13px;
  }
}
.active {
  background: #c00;
  color: #ff9;
}
</style>
