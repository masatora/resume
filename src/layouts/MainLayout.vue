<template>
  <div class="" style="padding-top: 60px">
    <div id="navigate">
      <a href="#PROFILE">PROFILE</a>
      <a href="#SKILL">SKILL</a>
      <a href="#PORTFOLIO">PORTFOLIO</a>
      <a href="#EXPERIENCE">EXPERIENCE</a>
      <a href="#CONTACT">CONTACT</a>
    </div>
    <a name="PROFILE" />
    <div class="row justify-between">
      <q-parallax>
        <template v-slot:media>
          <img src="nddw0kak6nq41.jpg">
        </template>
        <template v-slot:content="scope">
          <div class="absolute column items-center"
            :style="{
              opacity: 0.45 + (1 - scope.percentScrolled) * 0.55,
              top: (scope.percentScrolled * 60) + '%',
              left: 0,
              right: 0
            }"
          >
          <div style="width: 70%; border: 1px solid red">
            <p class="text-h3 text-center text-white">PROFILE</p>
            <div class="row">
              <div class="col">
                <img src="" />
              </div>
              <div class="col">
                <p class="text-body1 text-white">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              </div>
            </div>
          </div>
          </div>
        </template>
      </q-parallax>
    </div>
    <a name="SKILL" />
    <br />
    <div>
      <h3 class="text-center">SKILL</h3>
      <div class="flex justify-center">
        <div class="row q-gutter-md q-mb-md" style="width: 70%">
          <q-card class="col" flat bordered>
            <q-card-section>
              <div class="text-overline text-orange-9">Overline</div>
              <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
              <div class="text-caption text-grey">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </q-card-section>
            <q-card-actions>
              <q-btn flat color="dark" label="Share" />
              <q-btn flat color="primary" label="Book" />
              <q-space />
              <q-btn color="grey" round flat dense :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="expanded = !expanded" />
            </q-card-actions>
            <q-slide-transition>
              <div v-show="expanded">
                <q-separator />
                <q-card-section class="text-subitle2">
                  {{ lorem }}
                </q-card-section>
              </div>
            </q-slide-transition>
          </q-card>
          <q-card class="col" flat bordered>
            <q-card-section>
              <div class="text-overline text-orange-9">Overline</div>
              <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
              <div class="text-caption text-grey">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </q-card-section>
            <q-card-actions>
              <q-btn flat color="dark" label="Share" />
              <q-btn flat color="primary" label="Book" />
              <q-space />
              <q-btn color="grey" round flat dense :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="expanded = !expanded" />
            </q-card-actions>
            <q-slide-transition>
              <div v-show="expanded">
                <q-separator />
                <q-card-section class="text-subitle2">
                  {{ lorem }}
                </q-card-section>
              </div>
            </q-slide-transition>
          </q-card>
          <q-card class="col" flat bordered>
            <q-card-section>
              <div class="text-overline text-orange-9">Overline</div>
              <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
              <div class="text-caption text-grey">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </q-card-section>
            <q-card-actions>
              <q-btn flat color="dark" label="Share" />
              <q-btn flat color="primary" label="Book" />
              <q-space />
              <q-btn color="grey" round flat dense :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="expanded = !expanded" />
            </q-card-actions>
            <q-slide-transition>
              <div v-show="expanded">
                <q-separator />
                <q-card-section class="text-subitle2">
                  {{ lorem }}
                </q-card-section>
              </div>
            </q-slide-transition>
          </q-card>
        </div>
        <div class="row q-gutter-md" style="width: 70%">
          <q-card class="col" flat bordered>
            <q-card-section>
              <div class="text-overline text-orange-9">Overline</div>
              <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
              <div class="text-caption text-grey">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </q-card-section>
            <q-card-actions>
              <q-btn flat color="dark" label="Share" />
              <q-btn flat color="primary" label="Book" />
              <q-space />
              <q-btn color="grey" round flat dense :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="expanded = !expanded" />
            </q-card-actions>
            <q-slide-transition>
              <div v-show="expanded">
                <q-separator />
                <q-card-section class="text-subitle2">
                  {{ lorem }}
                </q-card-section>
              </div>
            </q-slide-transition>
          </q-card>
          <q-card class="col" flat bordered>
            <q-card-section>
              <div class="text-overline text-orange-9">Overline</div>
              <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
              <div class="text-caption text-grey">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </q-card-section>
            <q-card-actions>
              <q-btn flat color="dark" label="Share" />
              <q-btn flat color="primary" label="Book" />
              <q-space />
              <q-btn color="grey" round flat dense :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="expanded = !expanded" />
            </q-card-actions>
            <q-slide-transition>
              <div v-show="expanded">
                <q-separator />
                <q-card-section class="text-subitle2">
                  {{ lorem }}
                </q-card-section>
              </div>
            </q-slide-transition>
          </q-card>
          <q-card class="col" flat bordered>
            <q-card-section>
              <div class="text-overline text-orange-9">Overline</div>
              <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
              <div class="text-caption text-grey">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </div>
            </q-card-section>
            <q-card-actions>
              <q-btn flat color="dark" label="Share" />
              <q-btn flat color="primary" label="Book" />
              <q-space />
              <q-btn color="grey" round flat dense :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'" @click="expanded = !expanded" />
            </q-card-actions>
            <q-slide-transition>
              <div v-show="expanded">
                <q-separator />
                <q-card-section class="text-subitle2">
                  {{ lorem }}
                </q-card-section>
              </div>
            </q-slide-transition>
          </q-card>
        </div>
      </div>
    </div>
    <a name="PORTFOLIO" />
    <br />
    <div>
      <h3 class="text-center">PORTFOLIO</h3>
      <div class="flex justify-center">
        <div class="q-gutter-md" style="width: 70%">
          <q-card>
            <q-card-section horizontal>
              <q-img class="col-5" src="水利局1.png" />
              <q-card-section style="width: 100%">
                <q-list dense class="text-body1">
                  <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                  <q-item class="text-h6 text-bold flex justify-center">新北水利局雨水下水道水位監測系統</q-item>
                  <q-separator class="q-my-sm" />
                  <q-item class="text-bold">專案說明：</q-item>
                  <q-item>提供雨水下水道水位即時監測與資料分析，提升人員效率並即時處理淹水情況</q-item>
                  <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計，與 PM 協同規劃</q-item>
                  <q-item>．前端：ES6、Vue / Quasar、Cesium、Stylus</q-item>
                  <q-item>．後端：Python / Flask、MySQL、Nginx、Windows</q-item>
                  <q-item class="text-bold">專案特色：</q-item>
                  <q-item>．直覺式水位警戒辨識</q-item>
                  <q-item>．雨量與水位統計分析</q-item>
                  <q-item>．淹水示意及即時影像</q-item>
                  <q-item>．現場抽水設備監測</q-item>
                </q-list>
              </q-card-section>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" />
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://wrs.ntpc.thinktron.co/')" />
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal>
              <q-img class="col-5" src="水源局1.png" />
              <q-card-section style="width: 100%">
                <q-list dense class="text-body1">
                  <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                  <q-item class="text-h6 text-bold flex justify-center">新北市水源特定區智慧預報系統</q-item>
                  <q-separator class="q-my-sm" />
                  <q-item class="text-bold">專案說明：</q-item>
                  <q-item>提供山區崩塌預測，以避免發生災害時的人員傷亡及週邊設備財物損失</q-item>
                  <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計並支援手機版本操作，與 AI 工程師及 PM 協同合作開發</q-item>
                  <q-item>．前端：ES6、Vue / Quasar、Cesium、Stylus</q-item>
                  <q-item>．後端：Python / Flask、PostgreSQL、Redis、Nginx、Ubuntu</q-item>
                  <q-item class="text-bold">專案特色：</q-item>
                  <q-item>．各測站即時監測及資料分析</q-item>
                  <q-item>．各測站預測及資料分析</q-item>
                  <q-item>．直覺式的崩塌預警</q-item>
                  <q-item>．監測站警戒值圖像化</q-item>
                </q-list>
              </q-card-section>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" />
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://sss.wratb.gov.tw/')" />
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal>
              <q-img class="col-5" src="高爾夫1.png" />
              <q-card-section style="width: 100%">
                <q-list dense class="text-body1">
                  <q-badge class="absolute absolute-top-right text-body2 bg-grey" label="未維運" />
                  <q-item class="text-h6 text-bold flex justify-center">高爾夫球場自駕車派遣系統</q-item>
                  <q-separator class="q-my-sm" />
                  <q-item class="text-bold">專案說明：</q-item>
                  <q-item>減少球場雇用人力、自駕車自動化接送</q-item>
                  <q-item>．負責前後端圖台的程式設計、資料庫設計、 UI/UX 操作介面設計、MQTT Broker 及 WebSocket 串接並與合作廠商討論規格</q-item>
                  <q-item>．前端：ES6、Vue / Quasar、Stylus</q-item>
                  <q-item>．後端：Python / Flask、PostgreSQL、MQTT、Ubuntu</q-item>
                  <q-item class="text-bold">專案特色：</q-item>
                  <q-item>．透過 Web 技術對實體自駕車進行派遣</q-item>
                  <q-item>．自動規劃最佳路線</q-item>
                  <q-item>．車機發送 MQTT 資料到 Broker 後轉由 WebSocket 發送到客戶端以逹自駕車即時監控</q-item>
                  <q-item>．自駕車軌跡檢視、播放功能</q-item>
                  <q-item>．電子圍離系統</q-item>
                </q-list>
              </q-card-section>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" />
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://ysgolf.thinktron.co/')" />
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal>
              <q-img class="col-5" src="農糧署1.png" />
              <q-card-section style="width: 100%">
                <q-list dense class="text-body1">
                  <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                  <q-item class="text-h6 text-bold flex justify-center">農糧署農田判釋工作平台</q-item>
                  <q-separator class="q-my-sm" />
                  <q-item class="text-bold">專案說明：</q-item>
                  <q-item>利用 AI 辨識所選區域是否有潛在的可耕地</q-item>
                  <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計並與 AI 工程師配合開發</q-item>
                  <q-item>．前端：ES6、Vue / Quasar、Cesium、Stylus</q-item>
                  <q-item>．後端：Python / Flask、SQLite、Nginx、Ubuntu</q-item>
                  <q-item class="text-bold">專案特色：</q-item>
                  <q-item>．操作 web 介面來產生 AI 訓練結果，提昇用戶體驗</q-item>
                  <q-item>．視覺化可耕地位置及面積</q-item>
                  <q-item>．提供歷史查詢功能，以便驗証 AI 模型的準確性</q-item>
                </q-list>
              </q-card-section>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" />
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('http://103.124.73.17:8000/')" />
            </q-card-actions>
          </q-card>
          <q-card>
            <q-card-section horizontal>
              <q-img class="col-5" src="消防署1.png" />
              <q-card-section style="width: 100%">
                <q-list dense class="text-body1">
                  <q-badge class="absolute absolute-top-right text-body2 bg-positive" label="維運中" />
                  <q-item class="text-h6 text-bold flex justify-center">內政部消防署消防與救災數據分析系統平台</q-item>
                  <q-separator class="q-my-sm" />
                  <q-item class="text-bold">專案說明：</q-item>
                  <q-item>蒐集消防相關資料並進行資料清洗，再由 AI 團隊開發示警模組及輿情分析功能</q-item>
                  <q-item>．負責前後端程式設計、資料庫設計、 UI/UX 操作介面設計、資料清洗及壓力測試</q-item>
                  <q-item>．前端：ES6、Vue / Quasar、SASS</q-item>
                  <q-item>．後端：Python / FastAPI、PostgreSQL、Memcached、Nginx、Ubuntu、Beautiful Soup</q-item>
                  <q-item>．QA：JMeter</q-item>
                  <q-item class="text-bold">專案特色：</q-item>
                  <q-item>．視覺化監控爬蟲程式狀態</q-item>
                  <q-item>．詮釋資料審核管理</q-item>
                  <q-item>．API 資料開放介接</q-item>
                </q-list>
              </q-card-section>
            </q-card-section>
            <q-separator />
            <q-card-actions class="flex justify-end q-gutter-md">
              <q-btn color="blue-grey-5" flat round icon="movie" />
              <q-btn color="blue-grey-5" flat round icon="public" @click="openLink('https://nfadw.emic.gov.tw/')" />
            </q-card-actions>
          </q-card>
        </div>
      </div>
    </div>
    <a name="EXPERIENCE" />
    <br />
    <div class="flex justify-center">
      <div class="q-px-lg q-pb-md" style="width: 70%">
        <h3 class="text-center">EXPERIENCE</h3>
        <q-timeline color="secondary">
          <q-timeline-entry
            title="興創知能股份有限公司"
            subtitle="2019-05 ~ 至今"
            icon="psychology"
          >
            <div>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </div>
          </q-timeline-entry>
          <q-timeline-entry
            title="驊訊電子企業股份有限公司"
            subtitle="2017-09 ~ 2018-11"
            icon="memory"
          >
            <div>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </div>
          </q-timeline-entry>
          <q-timeline-entry
            title="新加坡商優達斯國際有限公司"
            subtitle="2014-01 ~ 2017-01"
            icon="shopping_cart"
          >
            <div>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </div>
          </q-timeline-entry>
          <q-timeline-entry
            title="宇峻奧汀科技股份有限公司"
            subtitle="2012-04 ~ 2013-06"
            icon="sports_esports"
          >
            <div>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </div>
          </q-timeline-entry>
        </q-timeline>
      </div>
    </div>
    <a name="CONTACT" />
    <br />
    <div class="">
      <h3 class="text-center">CONTACT</h3>
      <div class="flex justify-center q-gutter-xl q-py-xl">
        <q-btn icon="email" color="blue-grey-5" size="xl" flat round />
        <q-btn icon="phone" color="blue-grey-5" size="xl" flat round />
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
    onMounted(() => {
    })

    return {
      openLink,
      expanded: ref(false),
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    }
  }
})
</script>

<style lang="sass">
#navigate
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
  z-index: 10

  a
    cursor: pointer
    width: calc(100% / 5)
    height: 60px
    line-height: 60px
    font-size: 20px
    font-weigth: bolder
    text-align: center

  a:hover
    color: #000
    background-color: #F5F5F5

  a:visited
    color: #AAA

  a:link
    color: #AAA
    text-decoration: none

</style>
