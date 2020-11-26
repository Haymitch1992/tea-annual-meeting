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
      <div class="img-box">
        <el-row>
          <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
            <div class="video-box"></div>
            <dd class="zuzhi">
              <p>指导单位：中华全国供销合作总社</p>
              <br />
              <p>主办单位：中国茶叶流通协会</p>
              <p>云南省农业农村厅</p>
              <p>云南省供销合作社</p>
              <p>西双版纳傣族自治州人民政府</p>
              <br />
              <p>承办单位：勐海县人民政府、西双版纳州农业农村局</p>
              <br />
              <p>
                协办单位：全国各省级茶叶行业组织、云南省茶叶流通协会
              </p>
              <p>健康中国 科学饮茶 茶王勐海 世界之恋</p>
            </dd>
          </el-col>
          <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12">
            <div class="zixun-item">
              <h3>
                “第十五届中国茶业经济年会暨2019中国英德红茶文化节”盛大举行
              </h3>
              <p>
                金秋十月丹桂飘香，岭南古驿共襄盛举。10月22日上午，由中国茶叶流通协会、广东省农业农村厅、广东省供销合作联社、清远市人民政府联合主办，英德市人民政府、清远市农业农村局承办，全国各省级茶叶行业组织等单位协办的第十五届中国茶业经济年会暨2019中国英德红茶文化节，在广东省英德市举行了简朴、隆重、热烈的开幕式。<a
                  href=""
                  >详细>></a
                >
              </p>
            </div>
            <div class="zixun-item">
              <h3>
                “第十五届中国茶业经济年会暨2019中国英德红茶文化节”盛大举行
              </h3>
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
                  href="http://www.ctma.com.cn/ctma_news/2019nianhui/news/2019/1028/61300.html"
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
                  href="http://www.ctma.com.cn/ctma_news/2019nianhui/news/2019/1028/61299.html"
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
        </el-row>
      </div>
      <!--滚动轮播-->
      <div class="img-box">
        <td id="cflRollLeft1">
          <!--nr-->
          <table cellspacing="0" cellpadding="0" border="0">
            <tbody>
              <tr>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=1"
                            target="_blank"
                            >第十五届中国茶业经济年会<br />盛大开幕</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=2"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_02.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=2"
                            target="_blank"
                            >第十五届中国茶业经济年会<br />盛大开幕</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=15"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_15.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=15"
                            target="_blank"
                            >首长宣布开幕</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=17"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_17.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=17"
                            target="_blank"
                            >首长宣布开幕</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=8"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_08.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=8"
                            target="_blank"
                            >清远市委副书记、市长黄喜忠</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=11"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_11.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=11"
                            target="_blank"
                            >广东省人民政府副秘书长郑伟仪</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=13"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_13.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=13"
                            target="_blank"
                            >中华全国供销合作总社党组成员、理事会副主任王伟</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=4"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_04.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=4"
                            target="_blank"
                            >中国茶叶流通协会会长王庆</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=6"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_06.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=6"
                            target="_blank"
                            >第十五届中国茶业经济年会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=19"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_19.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=19"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=20"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_20.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=20"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=21"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_21.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=21"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=22"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_22.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=22"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=23"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_23.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=23"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=24"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_24.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=24"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=25"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_25.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=25"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=26"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_26.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=26"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=27"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_27.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=27"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=28"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_28.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=28"
                            target="_blank"
                            >授牌仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=29"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_29.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=29"
                            target="_blank"
                            >会旗交接仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=30"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/kms_30.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/kms.php?id=30"
                            target="_blank"
                            >会旗交接仪式</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hz.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/hz_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hz.php?id=1"
                            target="_blank"
                            >媒体采访</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hz.php?id=3"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/hz_03.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hz.php?id=3"
                            target="_blank"
                            >媒体采访</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/dsl.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/dsl_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/dsl.php?id=1"
                            target="_blank"
                            >大茶客沙龙</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/dsl.php?id=2"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/dsl_02.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/dsl.php?id=2"
                            target="_blank"
                            >大茶客沙龙</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=2"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/lsh_02.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=2"
                            target="_blank"
                            >六届三次理事会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=4"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/lsh_04.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=4"
                            target="_blank"
                            >六届三次理事会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=16"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/lsh_16.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=16"
                            target="_blank"
                            >六届三次理事会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=21"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/lsh_21.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/lsh.php?id=21"
                            target="_blank"
                            >六届三次理事会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/jsh.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191021/jsh_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/jsh.php?id=1"
                            target="_blank"
                            >第一届三次监事会会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/bgh.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/bgh_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/bgh.php?id=1"
                            target="_blank"
                            >主题报告会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/bgh.php?id=9"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/bgh_09.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/bgh.php?id=9"
                            target="_blank"
                            >主题报告会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/bgh.php?id=12"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/bgh_12.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/bgh.php?id=12"
                            target="_blank"
                            >主题报告会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/hclt_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=1"
                            target="_blank"
                            >首届国际红茶品牌发展论坛</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=2"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/hclt_02.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=2"
                            target="_blank"
                            >首届国际红茶品牌发展论坛</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=16"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/hclt_16.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=16"
                            target="_blank"
                            >首届国际红茶品牌发展论坛</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=17"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191022/hclt_17.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/hclt.php?id=17"
                            target="_blank"
                            >首届国际红茶品牌发展论坛</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zlaq_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=1"
                            target="_blank"
                            >中国茶叶质量安全新热点解析</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=4"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zlaq_04.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=4"
                            target="_blank"
                            >中国茶叶质量安全新热点解析</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=6"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zlaq_06.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=6"
                            target="_blank"
                            >中国茶叶质量安全新热点解析</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=7"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zlaq_07.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zlaq.php?id=7"
                            target="_blank"
                            >中国茶叶质量安全新热点解析</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zscq_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=1"
                            target="_blank"
                            >会员专题交流报告会——茶业知识产权保护</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=3"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zscq_03.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=3"
                            target="_blank"
                            >会员专题交流报告会——茶业知识产权保护</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=4"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zscq_04.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=4"
                            target="_blank"
                            >会员专题交流报告会——茶业知识产权保护</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=5"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zscq_05.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zscq.php?id=5"
                            target="_blank"
                            >会员专题交流报告会——茶业知识产权保护</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zwcxdj_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=1"
                            target="_blank"
                            >中外茶叶产销对接交流会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=2"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zwcxdj_02.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=2"
                            target="_blank"
                            >中外茶叶产销对接交流会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=3"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zwcxdj_03.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=3"
                            target="_blank"
                            >中外茶叶产销对接交流会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=4"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191023/zwcxdj_04.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/zwcxdj.php?id=4"
                            target="_blank"
                            >中外茶叶产销对接交流会</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>

                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=1"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191024/cgkc_01.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=1"
                            target="_blank"
                            >参观考察</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=6"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191024/cgkc_06.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=6"
                            target="_blank"
                            >参观考察</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=11"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191024/cgkc_11.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=11"
                            target="_blank"
                            >参观考察</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
                <td valign="top">
                  <table
                    width="100%"
                    cellspacing="0"
                    cellpadding="0"
                    border="0"
                  >
                    <tbody>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=12"
                            target="_blank"
                            ><img
                              src="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/thumbs2/20191024/cgkc_12.jpg"
                              width="200"
                              height="135"
                              border="0"
                          /></a>
                        </td>
                      </tr>
                      <tr valign="top">
                        <td align="center">
                          <a
                            href="http://www.ctma.com.cn/ctma_news/2019nianhui/slides/cgkc.php?id=12"
                            target="_blank"
                            >参观考察</a
                          >
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </td>
              </tr>
            </tbody>
          </table>
          <!--nr-->
        </td>
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
      <!--图片展示-->
      <div class="img-box">
        <div class="img-box-title">
          <h2>
            辉煌历程
          </h2>
        </div>
        <img
          src="http://www.ctma.com.cn/ctma_news/2019nianhui/map03.png"
          alt=""
        />
      </div>
      <!--图片展示-->
      <div class="img-box">
        <div class="img-box-title">
          <h2>
            年会举办地
          </h2>
        </div>

        <iframe
          src="http://www.ctma.com.cn/map.php?ac=2019nh"
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
  created: function() {
    var speedLeft = 20;
    cflRollLeft2.innerHTML = cflRollLeft1.innerHTML;
    function marqueeLeft() {
      if (cflRollLeft2.offsetWidth - cflRollLeft.scrollLeft <= 0)
        cflRollLeft.scrollLeft -= cflRollLeft1.offsetWidth;
      else {
        cflRollLeft.scrollLeft++;
      }
    }
    var myBarLeft = setInterval(marqueeLeft, speedLeft);
    cflRollLeft.onmouseover = function() {
      clearInterval(myBarLeft);
    };
    cflRollLeft.onmouseout = function() {
      myBarLeft = setInterval(marqueeLeft, speedLeft);
    };
    let num = 20;
    let dom = document.getElementById("cflRollLeft1");
    setInterval(() => {
      dom.style.left = dom.style.left + num;
    });
  },
};
</script>
<style scoped lang="scss">
.img-box {
  overflow: hidden;
  #cflRollLeft1 {
    text-align: left;
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
    padding: 0 10px;
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
      font-size: 14px;
    }
    a {
      color: #f60;
      padding: 0 10px;
      margin-left: 10px;
      font-size: 14px;
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
