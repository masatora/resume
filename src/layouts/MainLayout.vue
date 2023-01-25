<template>
  <div v-scroll="onScroll" style="padding-top: 60px">
    <div id="navDesktop" class="gt-xs">
      <a href="#PROFILE">PROFILE</a>
      <a href="#SKILLS">SKILLS</a>
      <a href="#PORTFOLIO">PORTFOLIO</a>
      <a href="#EXPERIENCE">EXPERIENCE</a>
      <a href="#CONTACT">CONTACT</a>
    </div>
    <div id="navMobile" class="lt-sm">
      <div class="row" style="height: 60px">
        <div class="col-2 flex justify-center">
          <q-btn icon="menu" size="lg" style="width: 100%" flat dense @click="isShowNavi = !isShowNavi" />
        </div>
        <div class="col text-h4 flex justify-center items-center">{{ positionName }}</div>
        <div class="col-2"></div>
      </div>
      <q-slide-transition>
        <q-list class="bg-white" v-show="isShowNavi" @click="isShowNavi = false">
          <q-item><a href="#PROFILE">PROFILE</a></q-item>
          <q-item><a href="#SKILLS">SKILLS</a></q-item>
          <q-item><a href="#PORTFOLIO">PORTFOLIO</a></q-item>
          <q-item><a href="#EXPERIENCE">EXPERIENCE</a></q-item>
          <q-item><a href="#CONTACT">CONTACT</a></q-item>
        </q-list>
      </q-slide-transition>
    </div>
    <a name="PROFILE" />
    <div class="row">
      <q-parallax :height="windowHeight">
        <template v-slot:media>
          <img src="https://picsum.photos/1920/1080">
        </template>
        <div class="row flex justify-center">
          <div class="col-xs-12 col-sm-10 col-md-8 col-lg-7" style="background-color: rgba(0, 0, 0, 0.3); border-radius: 10px">
            <p class="text-h3 text-bold text-center text-white q-pa-lg">PROFILE</p>
            <div class="row q-px-md">
              <div class="col-xs-12 col-md-6 flex justify-center" style="height: 34vmin">
                <img src="img/github-logo.png" style="max-width: 100%; max-height: 100%" />
              </div>
              <div class="col-xs-12 col-md-6 gt-xs text-body1">
                <p class="text-white">我對前端及後端均有濃厚興趣，也有扎實的開發歷練，從事全端開發工作已有近10年的經驗，專案的規劃設計、開發、部署及維運皆能獨力完成，並以全端工程師做為職涯方向。</p>
                <p class="text-white">透過自學掌握前端技術 HTML、Javascript / JQuery、CSS及切版技巧，設計出基於使用者角度思考的 UI/UX；後端方面技術則包含 PHP、MySQL 資料庫操作、SQL 查詢最佳化及效能調校。</p>
                <p class="text-white">在不同的工作歷練下也逐漸掌握了 Python、RESTful API、Vue、PostgreSQL、Web GIS 等各項技術，為業主服務也獲得優良評價，如內政部消防署、新北市水利局及水源特定區管理局等。</p>
                <p class="text-white">我喜歡學習各式框架與生態系，應用不同的技術來面對不斷變化的產業趨勢，我也樂於分享自己的開發經驗給予團隊，希望能以這份熱忱來鼓舞團隊並且一起成長!!</p>
              </div>
              <div class="col-xs-12 col-md-6 lt-sm text-body2">
                <p class="text-white">我對前端及後端均有濃厚興趣，也有扎實的開發歷練，從事全端開發工作已有近10年的經驗，專案的規劃設計、開發、部署及維運皆能獨力完成，並以全端工程師做為職涯方向。</p>
                <p class="text-white">透過自學掌握前端技術 HTML、Javascript / JQuery、CSS及切版技巧，設計出基於使用者角度思考的 UI/UX；後端方面技術則包含 PHP、MySQL 資料庫操作、SQL 查詢最佳化及效能調校。</p>
                <p class="text-white">在不同的工作歷練下也逐漸掌握了 Python、RESTful API、Vue、PostgreSQL、Web GIS 等各項技術，為業主服務也獲得優良評價，如內政部消防署、新北市水利局及水源特定區管理局等。</p>
                <p class="text-white">我喜歡學習各式框架與生態系，應用不同的技術來面對不斷變化的產業趨勢，我也樂於分享自己的開發經驗給予團隊，希望能以這份熱忱來鼓舞團隊並且一起成長!!</p>
              </div>
            </div>
          </div>
        </div>
      </q-parallax>
    </div>
    <a name="SKILLS" />
    <br />
    <div>
      <h3 class="text-bold text-center">SKILLS</h3>
      <div class="row flex justify-center">
        <div class="col-xs-12 col-sm-10 col-md-8 row">
          <div class="col-xs-12 col-md">
            <q-card class="q-mx-sm q-mb-sm" flat bordered>
              <q-card-section class="q-pb-none">
                <q-list class="text-body1 text-grey" dense>
                  <q-item-label class="text-h6 text-center q-my-sm text-orange-9">Front - End</q-item-label>
                  <q-item>Vue.js / Quasar / Vuex / Pinia</q-item>
                  <q-item>Cesium / leaflet</q-item>
                  <q-item>Javascript / JQuery / Ramda</q-item>
                  <q-item>CSS3 / SASS / Stylus</q-item>
                  <q-item>WindiCSS / Bootstrap</q-item>
                  <q-item>HTML5 / SPA / SSR / RWD</q-item>
                </q-list>
              </q-card-section>
              <q-card-actions class="flex justify-end q-py-none">
                <q-btn color="grey" round flat :icon="frontEndExpanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="frontEndExpanded = !frontEndExpanded" />
              </q-card-actions>
              <q-slide-transition>
                <div v-show="frontEndExpanded">
                  <q-separator />
                  <q-card-section class="text-body2">
                    熟悉網頁切版及 CSS 來設計 UI/UX 並能夠製作出響應式網頁或是套用前端框架來進行開發
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-xs-12 col-md">
            <q-card class="q-mx-sm q-mb-sm" flat bordered>
              <q-card-section class="q-pb-none">
                <q-list class="text-body1 text-grey" dense>
                  <q-item-label class="text-h6 text-center q-my-sm text-orange-9">Back - End</q-item-label>
                  <q-item>Python - Flask / FastAPI / Sanic</q-item>
                  <q-item>PHP - CodeIgniter</q-item>
                  <q-item>RESTful API</q-item>
                  <q-item>JWT / OAUTH</q-item>
                  <q-item>numpy / pandas</q-item>
                  <q-item>Beautiful soup 4</q-item>
                </q-list>
              </q-card-section>
              <q-card-actions class="flex justify-end q-py-none">
                <q-btn color="grey" round flat :icon="backEndExpanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="backEndExpanded = !backEndExpanded" />
              </q-card-actions>
              <q-slide-transition>
                <div v-show="backEndExpanded">
                  <q-separator />
                  <q-card-section class="text-body2">
                    後端採用 Restful API 風格進行開發，權限認證主要使用 JWT，熟稔各類加密與程式撰寫方法，以符合資安開發要求
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-xs-12 col-md">
            <q-card class="q-mx-sm q-mb-sm" flat bordered>
              <q-card-section class="q-pb-none">
                <q-list class="text-body1n text-grey" dense>
                  <q-item-label class="text-h6 text-center q-my-sm text-orange-9">Database</q-item-label>
                  <q-item>PostgreSQL / PostGIS / TimescaleDB</q-item>
                  <q-item>MySQL</q-item>
                  <q-item>SQLite</q-item>
                  <q-item>Oracle PL/SQL</q-item>
                  <q-item>Redis</q-item>
                  <q-item>Memcached</q-item>
                </q-list>
              </q-card-section>
              <q-card-actions class="flex justify-end q-py-none">
                <q-btn color="grey" round flat :icon="databaseExpanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="databaseExpanded = !databaseExpanded" />
              </q-card-actions>
              <q-slide-transition>
                <div v-show="databaseExpanded">
                  <q-separator />
                  <q-card-section class="text-body2">
                    在資料庫 Schema 的設計、查詢最佳化及效能調校有相當豐富經驗，也能夠運用空間資料及時序式資料庫
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
        </div>
        <div class="col-xs-12 col-sm-10 col-md-8 row">
          <div class="col-xs-12 col-md">
            <q-card class="q-mx-sm q-mt-sm" flat bordered>
              <q-card-section class="q-pb-none">
                <q-list class="text-body1 text-grey" dense>
                  <q-item-label class="text-h6 text-center q-my-sm text-orange-9">Environment</q-item-label>
                  <q-item>Windows</q-item>
                  <q-item>Ubuntu</q-item>
                  <q-item>Docker</q-item>
                  <q-item>VirtualBox</q-item>
                  <q-item>RaspberryPi / Arduino</q-item>
                </q-list>
              </q-card-section>
              <q-card-actions class="flex justify-end q-py-none">
                <q-btn color="grey" round flat :icon="osExpanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="osExpanded = !osExpanded" />
              </q-card-actions>
              <q-slide-transition>
                <div v-show="osExpanded">
                  <q-separator />
                  <q-card-section class="text-body2">
                    熟悉各開發環境建置及線上環境部署；另外也能夠製作電路搭配樹莓派或 Arduino 開發出 IoT 裝置
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-xs-12 col-md">
            <q-card class="q-mx-sm q-mt-sm" flat bordered>
              <q-card-section class="q-pb-none">
                <q-list class="text-body1 text-grey" dense>
                  <q-item-label class="text-h6 text-center q-my-sm text-orange-9">VCS</q-item-label>
                  <q-item>Git</q-item>
                  <q-item>Github</q-item>
                  <q-item>Gitlab</q-item>
                  <q-item>BitBucket</q-item>
                  <q-item>SVN</q-item>
                </q-list>
              </q-card-section>
              <q-card-actions class="flex justify-end q-py-none">
                <q-btn color="grey" round flat :icon="vcsExpanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="vcsExpanded = !vcsExpanded" />
              </q-card-actions>
              <q-slide-transition>
                <div v-show="vcsExpanded">
                  <q-separator />
                  <q-card-section class="text-body2">
                    瞭解基本 Git 指令並且能理解 Git Flow、Github Flow 及 Gitlab Flow 開發流程並運用在工作中
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-xs-12 col-md">
            <q-card class="q-mx-sm q-mt-sm" flat bordered>
              <q-card-section class="q-pb-none">
                <q-list class="text-body1 text-grey" dense>
                  <q-item-label class="text-h6 text-center q-my-sm text-orange-9">Other</q-item-label>
                  <q-item>Nginx</q-item>
                  <q-item>Apache</q-item>
                  <q-item>MQTT</q-item>
                  <q-item>JMeter</q-item>
                  <q-item></q-item>
                </q-list>
              </q-card-section>
              <q-card-actions class="flex justify-end q-py-none">
                <q-btn color="grey" round flat :icon="otherExpanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="otherExpanded = !otherExpanded" />
              </q-card-actions>
              <q-slide-transition>
                <div v-show="otherExpanded">
                  <q-separator />
                  <q-card-section class="text-body2">
                    工作中常使用的軟體，在操作及設定上能做最適當的配置
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
        </div>
      </div>
    </div>
    <a name="PORTFOLIO" />
    <br />
    <div>
      <h3 class="text-bold text-center">PORTFOLIO</h3>
      <div class="row flex justify-center">
        <div class="col-xs-12 col-sm-10 col-md-8 q-gutter-md">
          <q-card>
            <q-card-section horizontal v-if="golfVideo">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/水利局.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else>
              <div class="row" style="width: 100%">
                <div class="col-xs-12 col-md-5">
                  <q-card-section class="q-pa-none">
                    <q-carousel v-model="wrsSlide" animated arrows swipeable navigation infinite style="border-radius: 6px">
                      <q-carousel-slide :name="1" img-src="img/水利局1.png" />
                      <q-carousel-slide :name="2" img-src="img/水利局2.png" />
                      <q-carousel-slide :name="3" img-src="img/水利局3.png" />
                      <q-carousel-slide :name="4" img-src="img/水利局4.png" />
                      <q-carousel-slide :name="5" img-src="img/水利局5.png" />
                    </q-carousel>
                  </q-card-section>
                </div>
                <div class="col-xs-12 col-md-7">
                  <q-card-section>
                    <q-list dense class="text-body1">
                      <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                      <q-item class="text-h6 text-bold flex justify-center">新北市水利局雨水下水道水位監測系統</q-item>
                      <q-separator class="q-my-xs" />
                      <q-item class="text-bold">專案說明：</q-item>
                      <q-item>提供雨水下水道水位即時監測與資料分析，提升人員效率並即時處理淹水情況</q-item>
                      <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計，與 PM 協同規劃</q-item>
                      <q-item>．前端：ES6、Vue / Quasar、Cesium、Stylus、Highcharts</q-item>
                      <q-item>．後端：Python / Flask、MySQL、Geoserver、Nginx、Windows</q-item>
                      <q-item class="text-bold">專案特色：</q-item>
                      <q-item>．Highcharts 時序、統計資料視覺化</q-item>
                      <q-item>．Cesium Web GIS 與測站連動即時呈現水位狀況</q-item>
                      <q-item>．Requests 資料介接並整合各機關 API，實現影像串接服務及即時淹水警示</q-item>
                    </q-list>
                  </q-card-section>
                </div>
              </div>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" @click="wrsVideo = !wrsVideo">
                <q-tooltip>水利局 DEMO</q-tooltip>
              </q-btn>
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://wrs.ntpc.thinktron.co/')">
                <q-tooltip>開啟網頁</q-tooltip>
              </q-btn>
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal v-if="wratbVideo1">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/水源局1.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else-if="wratbVideo2">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/水源局2.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else>
              <div class="row" style="width: 100%">
                <div class="col-xs-12 col-md-5">
                  <q-card-section class="q-pa-none">
                    <q-carousel v-model="wratbSlide" animated arrows swipeable navigation infinite style="border-radius: 6px">
                      <q-carousel-slide :name="1" img-src="img/水源局1.png" />
                      <q-carousel-slide :name="2" img-src="img/水源局2.png" />
                      <q-carousel-slide :name="3" img-src="img/水源局3.png" />
                      <q-carousel-slide :name="4" img-src="img/水源局4.png" />
                      <q-carousel-slide :name="5" img-src="img/水源局5.png" />
                    </q-carousel>
                  </q-card-section>
                </div>
                <div class="col-xs-12 col-md-7">
                  <q-card-section>
                    <q-list dense class="text-body1">
                      <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                      <q-item class="text-h6 text-bold flex justify-center">新北市水源特定區智慧預報系統</q-item>
                      <q-separator class="q-my-xs" />
                      <q-item class="text-bold">專案說明：</q-item>
                      <q-item>提供山區崩塌預測，避免發生災害時人員傷亡或週邊設備財物損失</q-item>
                      <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計並支援手機版本操作，與 AI 工程師及 PM 協同合作開發</q-item>
                      <q-item>．前端：ES6、Vue / Quasar、Cesium、Stylus、Highcharts</q-item>
                      <q-item>．後端：Python / Flask、PostgreSQL、Redis、Nginx、Ubuntu</q-item>
                      <q-item class="text-bold">專案特色：</q-item>
                      <q-item>．氣象資源 API 整合與介接，提供即時觀測、預報及資料分析</q-item>
                      <q-item>．Quasar Framework 設計視覺化元件及符合各式設備的 RWD 版型</q-item>
                      <q-item>．Cesium 介接崩塌預測 API 實現崩塌預警</q-item>
                      <q-item>．Redis 實現資料備援機制，提升資料介接的穩定性</q-item>
                    </q-list>
                  </q-card-section>
                </div>
              </div>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" @click="wratbVideo1 = false; wratbVideo2 = !wratbVideo2">
                <q-tooltip>水源局 DEMO 2</q-tooltip>
              </q-btn>
              <q-btn color="blue-grey-5" flat round icon="movie" @click="wratbVideo2 = false; wratbVideo1 = !wratbVideo1">
                <q-tooltip>水源局 DEMO 1</q-tooltip>
              </q-btn>
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://sss.wratb.gov.tw/')">
                <q-tooltip>開啟網頁</q-tooltip>
              </q-btn>
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal v-if="golfVideo">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/高爾夫.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else>
              <div class="row" style="width: 100%">
                <div class="col-xs-12 col-md-5">
                  <q-card-section class="q-pa-none">
                    <q-carousel v-model="golfSlide" animated arrows swipeable navigation infinite style="border-radius: 6px">
                      <q-carousel-slide :name="1" img-src="img/高爾夫1.png" />
                      <q-carousel-slide :name="2" img-src="img/高爾夫2.png" />
                      <q-carousel-slide :name="3" img-src="img/高爾夫3.png" />
                      <q-carousel-slide :name="4" img-src="img/高爾夫4.png" />
                      <q-carousel-slide :name="5" img-src="img/高爾夫5.png" />
                    </q-carousel>
                  </q-card-section>
                </div>
                <div class="col-xs-12 col-md-7">
                  <q-card-section>
                    <q-list dense class="text-body1">
                      <q-badge class="absolute absolute-top-right text-body2 bg-grey" label="未維運" />
                      <q-item class="text-h6 text-bold flex justify-center">高爾夫球場自駕車派遣系統</q-item>
                      <q-separator class="q-my-xs" />
                      <q-item class="text-bold">專案說明：</q-item>
                      <q-item>減少球場雇用人力、自駕車自動化接送</q-item>
                      <q-item>．負責前後端圖台的程式設計、資料庫設計、 UI/UX 操作介面設計、MQTT Broker 及 WebSocket 串接並與合作廠商討論規格</q-item>
                      <q-item>．前端：ES6、Vue / Quasar、Vuex、Cesium、Stylus、Highcharts、Websocket</q-item>
                      <q-item>．後端：Python / Flask、PostgreSQL、PostGIS、MQTT、Websocket、Ubuntu</q-item>
                      <q-item class="text-bold">專案特色：</q-item>
                      <q-item>．MQTT + WS 雙向溝通接收車機訊號，實現車輛定位與即時影像監控</q-item>
                      <q-item>．PostGIS 處理車機運行軌跡再處理成 CZML，由 Cesium 播放歷史軌跡記錄</q-item>
                      <q-item>．Cesium 繪製車道屏蔽範圍，再以 MQTT 發送至車機實現電子圍籬系統</q-item>
                    </q-list>
                  </q-card-section>
                </div>
              </div>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" @click="golfVideo = !golfVideo">
                <q-tooltip>高爾夫 DEMO</q-tooltip>
              </q-btn>
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://ysgolf.thinktron.co/')">
                <q-tooltip>開啟網頁</q-tooltip>
              </q-btn>
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal v-if="afaVideo">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/農糧署.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else>
              <div class="row" style="width: 100%">
                <div class="col-xs-12 col-md-5">
                  <q-card-section class="q-pa-none">
                    <q-carousel v-model="afaSlide" animated arrows swipeable navigation infinite style="border-radius: 6px">
                      <q-carousel-slide :name="1" img-src="img/農糧署1.png" />
                      <q-carousel-slide :name="2" img-src="img/農糧署2.png" />
                      <q-carousel-slide :name="3" img-src="img/農糧署3.png" />
                      <q-carousel-slide :name="4" img-src="img/農糧署4.png" />
                      <q-carousel-slide :name="5" img-src="img/農糧署5.png" />
                    </q-carousel>
                  </q-card-section>
                </div>
                <div class="col-xs-12 col-md-7">
                  <q-card-section>
                    <q-list dense class="text-body1">
                      <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                      <q-item class="text-h6 text-bold flex justify-center">農糧署農田判釋工作平台</q-item>
                      <q-separator class="q-my-xs" />
                      <q-item class="text-bold">專案說明：</q-item>
                      <q-item>利用 AI 辨識所選區域是否有潛在的可耕地</q-item>
                      <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計並與 AI 工程師配合開發</q-item>
                      <q-item>．前端：ES6、Vue / Quasar、Cesium、Stylus</q-item>
                      <q-item>．後端：Python / Flask、SQLite、Nginx、Ubuntu</q-item>
                      <q-item class="text-bold">專案特色：</q-item>
                      <q-item>．Axios 串接系統 AI 程式，提供視覺化操作與提昇用戶體驗</q-item>
                      <q-item>．Cesium Web GIS 圖層介接，視覺化可耕地位置及面積</q-item>
                      <q-item>．SQLite 紀錄 AI 運作結果，提供部署便利性</q-item>
                    </q-list>
                  </q-card-section>
                </div>
              </div>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" @click="afaVideo = !afaVideo">
                <q-tooltip>農糧署 DEMO</q-tooltip>
              </q-btn>
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('http://103.124.73.17:8000/')">
                <q-tooltip>開啟網頁</q-tooltip>
              </q-btn>
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal v-if="nfaVideo">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/消防署.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else>
              <div class="row" style="width: 100%">
                <div class="col-xs-12 col-md-5">
                  <q-card-section class="q-pa-none">
                    <q-carousel v-model="nfaSlide" animated arrows swipeable navigation infinite style="border-radius: 6px">
                      <q-carousel-slide :name="1" img-src="img/消防署1.png" />
                      <q-carousel-slide :name="2" img-src="img/消防署2.png" />
                      <q-carousel-slide :name="3" img-src="img/消防署3.png" />
                      <q-carousel-slide :name="4" img-src="img/消防署4.png" />
                    </q-carousel>
                  </q-card-section>
                </div>
                <div class="col-xs-12 col-md-7">
                  <q-card-section>
                    <q-list dense class="text-body1">
                      <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                      <q-item class="text-h6 text-bold flex justify-center">內政部消防署消防與救災數據分析系統平台</q-item>
                      <q-separator class="q-my-xs" />
                      <q-item class="text-bold">專案說明：</q-item>
                      <q-item>蒐集消防相關資料並進行資料清洗，再由 AI 團隊開發示警模組及輿情分析功能</q-item>
                      <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計、資料清洗及壓力測試</q-item>
                      <q-item>．前端：ES6、Vue / Quasar、SASS</q-item>
                      <q-item>．後端：Python / FastAPI、PostgreSQL、Memcached、Nginx、Beautiful Soup4</q-item>
                      <q-item>．QA：JMeter</q-item>
                      <q-item class="text-bold">專案特色：</q-item>
                      <q-item>．PostgreSQL 搭配系統排程，開發出爬蟲狀態即時監控視覺化架構</q-item>
                      <q-item>．BS4 做爬蟲開發，正規表達式進行資料清洗後儲存進資料倉儲</q-item>
                      <q-item>．Fastapi 開發出外部介接 API 再以 Swagger 發佈，以 JWT 做身份認證</q-item>
                    </q-list>
                  </q-card-section>
                </div>
              </div>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" @click="nfaVideo = !nfaVideo">
                <q-tooltip>消防署 DEMO</q-tooltip>
              </q-btn>
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://nfadw.emic.gov.tw/')">
                <q-tooltip>開啟網頁</q-tooltip>
              </q-btn>
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal v-if="nfaVideo">
              <video style="width: 100%; height: 100%" autoplay loop muted>
                <source type="video/mp4" src="video/農業局.mp4">
              </video>
            </q-card-section>
            <q-card-section horizontal v-else>
              <div class="row" style="width: 100%">
                <div class="col-xs-12 col-md-5">
                  <q-card-section class="q-pa-none">
                    <q-carousel v-model="nfaSlide" animated arrows swipeable navigation infinite style="border-radius: 6px">
                      <q-carousel-slide :name="1" img-src="img/農業局1.png" />
                      <q-carousel-slide :name="2" img-src="img/農業局2.png" />
                      <q-carousel-slide :name="3" img-src="img/農業局3.png" />
                      <q-carousel-slide :name="4" img-src="img/農業局4.png" />
                      <q-carousel-slide :name="5" img-src="img/農業局5.png" />
                      <q-carousel-slide :name="6" img-src="img/農業局6.png" />
                    </q-carousel>
                  </q-card-section>
                </div>
                <div class="col-xs-12 col-md-7">
                  <q-card-section>
                    <q-list dense class="text-body1">
                      <q-badge class="absolute absolute-top-right text-body2 bg-primary" label="開發中" />
                      <q-item class="text-h6 text-bold flex justify-center">新北市水土保持申請書件線上無紙化審查及管理系統</q-item>
                      <q-separator class="q-my-xs" />
                      <q-item class="text-bold">專案說明：</q-item>
                      <q-item>配合國家發展委員會電子化政府計畫，建立水土保持案件之管理、表單填寫及案件資料分析之功能</q-item>
                      <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計、簽核系統開發、資料電子化流程、應用程式虛擬化</q-item>
                      <q-item>．前端：ES6、Vue3 / Quasar、Pinia、SASS、WindiCSS、Cesium、Highcharts</q-item>
                      <q-item>．後端：Python / Sanic、JWT、PostgreSQL、Nginx</q-item>
                      <q-item>．DevOps：docker、Drone CI</q-item>
                      <q-item class="text-bold">專案特色：</q-item>
                      <q-item>．採用 Pinia 做為 vue3 做狀態管理工具，使開發易於維護且語法更為簡潔。</q-item>
                      <q-item>．CSS 框架採用 WindiCSS 以便於 UI/UX 設計、layout 等開發。</q-item>
                      <q-item>．採用 Sanic 後端框架，以提供響應時間更快速的 API 服務。</q-item>
                      <q-item>．應用程式使用 docker 做虛擬化，並利用 Drone CI 搭配 github 製作出易於部署的線上環境。</q-item>
                    </q-list>
                  </q-card-section>
                </div>
              </div>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" @click="nfaVideo = !nfaVideo">
                <q-tooltip>農業局 DEMO</q-tooltip>
              </q-btn>
            </q-card-actions>
          </q-card>
        </div>
      </div>
    </div>
    <a name="EXPERIENCE" />
    <br />
    <div class="row flex justify-center">
      <div class="col-xs-12 col-sm-10 col-md-8 q-px-md">
        <h3 class="text-bold text-center">EXPERIENCE</h3>
        <q-timeline color="secondary">
          <q-timeline-entry
            title="興創知能股份有限公司"
            subtitle="2019-05 ~ 至今"
            icon="psychology"
          >
            <q-list dense class="text-body1">
              <q-item-label class="text-bold q-py-sm">職稱</q-item-label>
              <q-item>全端軟體工程師</q-item>
              <q-item-label class="text-bold q-py-sm">工作內容</q-item-label>
              <q-item>1．專案開發: 主要工作項目為前後端程式開發，前端使用 Vue/Quasar 進行版型設計、切版與 API 串接，後端以 python 開發 Restful API、postgreSQL 資料庫設計、伺服器維運。專案內容多與 AIoT 有關並與團隊一起合作開發，將收到的 sensor 資料經由 AI 訓練，再將結果展示在 3D / 2D 空間圖台。</q-item>
              <q-item>2．網路維運: 兼任公司 MIS 工作，負責公司網路故障排除、伺服器維運等等。</q-item>
              <q-item>3．技術指導: 在 Web 方面有較多的開發經驗，因此在公司內也擔任技術方面的指導者。</q-item>
              <q-item-label class="text-bold q-py-sm">專案成果</q-item-label>
              <q-item>1．新北水利局雨水下水道水位監測系統</q-item>
              <q-item>2．新北市水源特定區崩塌預測系統</q-item>
              <q-item>3．高爾夫球場自駕車派遣系統</q-item>
              <q-item>4．農糧署農田判釋工作平台</q-item>
              <q-item>5．內政部消防署消防與救災數據分析系統平台</q-item>
              <q-item>6．巨量遙測空間數據AI分析雲端服務平台</q-item>
              <q-item>7．新北市水土保持申請書件線上無紙化審查及管理系統</q-item>
              <q-item-label class="text-bold q-py-sm">競賽成果</q-item-label>
              <q-item>1．2019 亞洲資料創新應用大擂台賽：臺灣研發獎勵獎</q-item>
              <q-item>2．2020 亞洲資料創新應用大擂台賽：Taiwan區最佳人氣獎第三名</q-item>
            </q-list>
          </q-timeline-entry>
          <q-timeline-entry
            title="驊訊電子企業股份有限公司"
            subtitle="2017-09 ~ 2018-11"
            icon="memory"
          >
            <q-list dense class="text-body1">
              <q-item-label class="text-bold q-py-sm">職稱</q-item-label>
              <q-item>Server軟體工程師</q-item>
              <q-item-label class="text-bold q-py-sm">工作內容</q-item-label>
              <q-item>1．後台歌曲管理系統開發及維護: PHP 與 MySQL 開發後台管理系統，利用 Git Flow 來控制開發進度，測試時以 JMeter 進行白箱測試，提升源始碼質量以保證後台功能的可用性</q-item>
              <q-item>2．開發視覺化營運報表: 以 Chart.js 將篩選的資料以視覺化來呈現與分析，綁定事件與客戶端互動。</q-item>
            </q-list>
          </q-timeline-entry>
          <q-timeline-entry
            title="新加坡商優達斯國際有限公司"
            subtitle="2014-01 ~ 2017-01"
            icon="shopping_cart"
          >
            <q-list dense class="text-body1">
              <q-item-label class="text-bold q-py-sm">職稱</q-item-label>
              <q-item>Web工程師</q-item>
              <q-item-label class="text-bold q-py-sm">工作內容</q-item-label>
              <q-item>1．開發維護電子商務網站前後台: PHP(CodeIgniter) 及 Oracle PL/SQL 來開發電商網站服務，以 MVC 架構進行開發。</q-item>
              <q-item>2．最佳化 SEO: 參照 schema.org 加入結構化資訊，並調整 DOM 結構與 HTML tag 使其更符合 SEO 語意，完成後在 google 的 1~3 頁之間皆能得出搜尋結果。</q-item>
              <q-item>3．程式效能分析與重構: 以 XHProf 進行源始碼效能測試，評估後以 SOLID 開發原則做為主軸，並著重於高內聚低耦合來進行重構，完成後再次進行測試效能提升了50%。</q-item>
              <q-item>4．資料庫查詢最佳化: 優化暨有 SQL statement 以 Explain Plan 進行分析，調整出最合適的語法以降低響應時間。</q-item>
            </q-list>
          </q-timeline-entry>
          <q-timeline-entry
            title="宇峻奧汀科技股份有限公司"
            subtitle="2012-04 ~ 2013-06"
            icon="sports_esports"
          >
            <q-list dense class="text-body1">
              <q-item-label class="text-bold q-py-sm">職稱</q-item-label>
              <q-item>Web程式設計</q-item>
              <q-item-label class="text-bold q-py-sm">工作內容</q-item-label>
              <q-item>1．遊戲官網建置維運: 前端以 JQuery 及 CSS 設計 UI 行為與樣式，後端為 php / VB.net 及 MySQL 來開發前台遊戲官網及後台管理系統，後台提供權限管理及訊息發佈等功能，將訊息呈現在前台上。</q-item>
              <q-item>2．遊戲獎勵兌換網頁活動開發: 前台設計遊戲活動，以 AJAX 串接 FB API 或遊戲內部 API 來兌換遊戲中的獎勵。</q-item>
              <q-item>3．技術研究: 將所有 .Net Framework 的官網移植至 Linux 上，並透過 Mono Framework 來完成，以減低在 Windows 上維運的成本。</q-item>
              <q-item>4．開發工具: 利用 SVN 開發出部門內程式自動上版流程，提升部門工作效率。</q-item>
            </q-list>
          </q-timeline-entry>
        </q-timeline>
      </div>
    </div>
    <a name="CONTACT" />
    <br />
    <div id="contact" class="col-12">
      <h3 class="text-bold text-center">CONTACT</h3>
      <div class="flex justify-center bg-blue-grey-1">
        <q-list>
          <q-item class="q-pa-lg" clickable @click="clickHref('https://github.com/masatora', '_blank')">
            <q-item-section side>
              <q-icon name="img:img/github.png" color="blue-grey-5" size="xl" />
            </q-item-section>
            <q-item-section class="text-body1">Github: https://github.com/masatora</q-item-section>
          </q-item>
          <q-item class="q-pa-lg" clickable @click="clickHref('mailto:omadedou@gmail.com')">
            <q-item-section side>
              <q-icon name="email" color="blue-grey-9" size="xl" />
            </q-item-section>
            <q-item-section class="text-body1">Email: omadedou@gmail.com</q-item-section>
          </q-item>
          <q-item class="q-pa-lg" clickable @click="clickHref('tel:+886-987220607')">
            <q-item-section side>
              <q-icon name="phone" color="blue-grey-9" size="xl" />
            </q-item-section>
            <q-item-section class="text-body1">Phone: 0987-220-607</q-item-section>
          </q-item>
        </q-list>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent, onMounted, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',
  components: {
  },

  setup () {
    const openLink = (link) => {
      window.open(link)
    }
    const clickHref = (href, target) => {
      const a = document.createElement('a')

      if (target !== undefined) {
        a.target = target
      }

      a.href = href
      a.click()
    }
    const windowHeight = ref(400)
    const positionName = ref('PROFILE')
    const skillsPos = ref({})
    const portfolioPos = ref({})
    const experiencePos = ref({})
    const contactPos = ref({})
    const onScroll = (position) => {
      if (contactPos.value.y <= position) {
        positionName.value = 'CONTACT'
      } else if (experiencePos.value.y <= position) {
        positionName.value = 'EXPERIENCE'
      } else if (portfolioPos.value.y <= position) {
        positionName.value = 'PORTFOLIO'
      } else if (skillsPos.value.y <= position) {
        positionName.value = 'SKILLS'
      } else {
        positionName.value = 'PROFILE'
      }
    }

    onMounted(async () => {
      windowHeight.value = (window.innerHeight * 4) / 5
      skillsPos.value = (document.getElementsByName('SKILLS')[0]).getBoundingClientRect()
      portfolioPos.value = (document.getElementsByName('PORTFOLIO')[0]).getBoundingClientRect()
      experiencePos.value = (document.getElementsByName('EXPERIENCE')[0]).getBoundingClientRect()
      contactPos.value = (document.getElementsByName('CONTACT')[0]).getBoundingClientRect()
    })

    return {
      isShowNavi: ref(false),
      wrsSlide: ref(1),
      wratbSlide: ref(1),
      golfSlide: ref(1),
      afaSlide: ref(1),
      nfaSlide: ref(1),
      wrsVideo: ref(false),
      wratbVideo1: ref(false),
      wratbVideo2: ref(false),
      golfVideo: ref(false),
      afaVideo: ref(false),
      nfaVideo: ref(false),
      frontEndExpanded: ref(false),
      backEndExpanded: ref(false),
      databaseExpanded: ref(false),
      osExpanded: ref(false),
      vcsExpanded: ref(false),
      otherExpanded: ref(false),
      windowHeight,
      positionName,
      openLink,
      onScroll,
      clickHref
    }
  }
})
</script>

<style lang="sass">
#navDesktop
  display: flex
  flex-wrap: wrap
  justify-content: space-evenly
  align-content: center
  position: fixed
  top: 0
  left: 0
  width: 100%
  height: 60px
  background-color: white
  z-index: 1

  a
    cursor: pointer
    width: calc(100% / 5)
    height: 60px
    line-height: 60px
    font-size: 20px
    font-weigth: bolder
    text-align: center
    text-decoration: none

  a:link
    color: #AAA

  a:visited
    color: #AAA

  a:hover
    color: #000
    background-color: #F5F5F5

  a:active
    color: #000

#navMobile
  position: fixed
  top: 0
  left: 0
  width: 100%
  height: 60px
  background-color: white
  z-index: 10

  a
    width: 100%
    font-size: 20px
    font-weigth: bolder
    text-align: center
    text-decoration: none

  a:link
    color: #AAA

  a:visited
    color: #AAA

  a:hover
    color: #000
    background-color: #F5F5F5

  a:active
    color: #000

#contact
  .flex
    padding: 100px 0 620px 0

  a
    text-decoration: none

</style>
