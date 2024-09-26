<template>
  <div class="child full rounded-u-l-2 nasalization container">
    <div class="child full rounded-2">
      <div class="child full container q-pa-none q-pt-xs rounded-u-l-1">
        <!-- UPWARDS CONTROL STATION -->
        <div class="child rounded-u-l-1 q-px-sm container">
          <q-btn-group flat push spread
            class="rounded-u-l-1 bg-orange-1 text-grey-8 q-pa-none q-my-xs">
            <q-btn push class="blue-borders q-pb-sm q-px-sm"
            size="0.6em" style="min-width:70%">
              <div class="ellipsis q-px-sm bg-brown-2 rounded-borders rounded-u-l-1">
                <q-icon name="account_tree"/> ::
  paths/c0f9d300e1b28253455e1835f13ca133152a6a9a9b106d0400980980980980980980980980980980980
              </div>
            </q-btn>
            <q-btn push class="blue-borders q-pb-sm text-blue-8" icon="content_paste"
              size="0.6em" />
            <q-btn push class="blue-borders q-pb-sm text-red-8" icon="push_pin" size="0.6em" />
            <q-btn push class="blue-borders q-pb-sm text-teal-8" icon="save" size="0.6em" />
            <q-btn push class="blue-borders q-pb-sm" icon="more_vert" size="0.6em" />
          </q-btn-group>
        </div>
        <!-- DOWNWARDS CONTROL STATION -->
        <div class="child q-mb-sm q-px-sm">
          <q-btn-group flat push
            class="bg-orange-1 rounded-b-1 text-grey-8 q-pa-none full-width">
            <q-btn push class="blue-borders full-width" size="sm" icon="route" />
            <q-btn push class="blue-borders full-width" size="sm" label="PATH" />
            <q-btn push class="blue-borders full-width" size="sm" icon="content_paste" />
            <q-btn push class="blue-borders full-width" size="sm" icon="push_pin" />
          </q-btn-group>
        </div>
        <!-- q-separator horizontal color="grey-5"/-->
        <!-- Noise box -->
        <div class="child full  container">
            <div class="child full q-pa-none container">
              <q-carousel
                v-model="slide"
                transition-prev="scale"
                transition-next="scale"
                swipeable
                animated
                control-color="grey-8"
                navigation
                arrows
                class="full q-px-xl q-pt-xs q-pb-xl transparent q-pa-none"
              >
                <q-carousel-slide name="style"
                  class="column no-wrap q-pa-none bg-orange-1 rounded-66 blue-borders flex-center">

                  <div class="column full thick-glass
                   no-wrap rounded-66 q-pa-none flex-center text-grey-8">
                    <div class="column full no-wrap rounded-66
                      flex-center text-grey-8">
                      <div class="col-1 full-width rounded-u-1">

                      </div>
                      <div class="col-11 full-width rounded-b-1 center">

                      </div>
                    </div>
                  </div>
                </q-carousel-slide>
                <q-carousel-slide name="tv" class="column no-wrap flex-center">
                  <q-icon name="music_note" size="156px" />
                  <div class="q-mt-md text-center">
                    {{ lorem }}
                  </div>
                </q-carousel-slide>
                <q-carousel-slide name="layers" class="column no-wrap flex-center">
                  <q-icon name="play_circle" size="156px" />
                  <div class="q-mt-md text-center">
                    {{ lorem }}
                  </div>
                </q-carousel-slide>
                <q-carousel-slide name="read" class="column no-wrap flex-center">
                  <q-icon name="menu_book" size="156px" />
                  <div class="q-mt-md text-center">
                    {{ lorem }}
                  </div>
                </q-carousel-slide>
              </q-carousel>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref, defineComponent } from 'vue';

export default defineComponent({
  name: 'NodeBox',
  setup() {
    return {
      slide: ref('style'),
      lorem: 'Insanus Contentus',
    };
  },
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
