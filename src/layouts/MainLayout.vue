<template>
  <div class="">
    <div class="row justify-between">
      <q-parallax>
        <template v-slot:media>
          <img src="nddw0kak6nq41.jpg">
        </template>
        <template v-slot:content="scope">
          <div
            class="absolute column items-center"
            :style="{
              opacity: 0.45 + (1 - scope.percentScrolled) * 0.55,
              top: (scope.percentScrolled * 60) + '%',
              left: 0,
              right: 0
            }"
          >
          <div>
            <p class="text-h3 text-white">簡介</p>
          </div>
          </div>
        </template>
      </q-parallax>
    </div>
    <div class="">
      <p class="text-h3 q-pa-md">工作技能</p>
      <q-card class="my-card" flat bordered>
        <q-img
          src="https://cdn.quasar.dev/img/parallax2.jpg"
        />

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

          <q-btn
            color="grey"
            round
            flat
            dense
            :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
            @click="expanded = !expanded"
          />
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
    <div>
      <p class="text-h3 q-pa-md">專案成就</p>
      <q-card class="my-card">
        <q-card-section horizontal>
          <q-img
            class="col-5"
            src="https://cdn.quasar.dev/img/parallax1.jpg"
          />

          <q-card-section>
            {{ lorem }}
          </q-card-section>
        </q-card-section>

        <q-separator />

        <q-card-actions>
          <q-btn flat round icon="event" />
          <q-btn flat>
            5:30PM
          </q-btn>
          <q-btn flat>
            7:00PM
          </q-btn>
          <q-btn flat color="primary">
            Reserve
          </q-btn>
        </q-card-actions>
      </q-card>
    </div>
    <div class="q-px-lg q-pb-md">
      <q-timeline color="secondary">
        <q-timeline-entry heading>工作經歷</q-timeline-entry>
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
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',
  components: {
  },
  setup () {
    return {
      expanded: ref(false),
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    }
  }
})
</script>
