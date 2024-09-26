<template>
  <div class="child full container blue-borders rounded-2">
    <q-splitter
      v-model="insideModel"
      separator-class="transparent"
      separator-style="height: 6px"
      class="child full rounded-2 q-pa-xs"
      horizontal
      style="height: 50em;"
    >

      <template v-slot:before>
        <q-splitter
          v-model="splitterModelA"
          separator-class="transparent"
          separator-style="width: 6px"
          class="child full rounded-2"
          style="height: 64em; max-height: 100%"
        >
        <template v-slot:before>
            <div class="full blue-surface rounded-u-l-2 container">
              <div class="full child q-pa-none rounded-u-l-2">
                <MainContainer></MainContainer>
              </div>
            </div>
          </template>

          <template v-slot:separator>
            <q-avatar round text-color="grey-8" color="lime-3" size="sm"
                      icon="grain" class="q-pa-none shadow-2 center"/>
          </template>

          <template v-slot:after>
            <div class="full red-surface rounded-u-r-2 container">
              <div class="full child q-pa-sm light-glass blue-borders rounded-u-r-2">
                <ContextContainer></ContextContainer>
              </div>
            </div>
          </template>
        </q-splitter>
      </template>

      <template v-slot:separator>
        <q-avatar round text-color="grey-8" color="yellow-3" size="sm"
                  icon="grain" class="q-pa-none shadow-2 center"/>
      </template>

      <template v-slot:after>
        <q-splitter
          v-model="splitterModelB"
          separator-class="transparent"
          separator-style="width: 6px"
          style="height: 64em; max-height: 100%"
        >
        <template v-slot:before>
            <div class="full red-surface-bottom rounded-b-2 container">
              <div class="full child q-pa-sm light-glass blue-borders rounded-b-2 ">
                <ContextContainer></ContextContainer>
              </div>
            </div>
          </template>

          <template v-slot:separator>
            <q-avatar round text-color="grey-8" color="orange-3" size="sm"
                      icon="grain" class="q-pa-none shadow-2 center"/>
          </template>

          <template v-slot:after>
            <div class="full red-surface-bottom rounded-b-2 container">
              <div class="full child q-pa-sm light-glass blue-borders rounded-b-2">
                <ContextContainer></ContextContainer>
              </div>
            </div>
          </template>
        </q-splitter>
      </template>

    </q-splitter>
  </div>
</template>

<script>
import { defineComponent, ref } from 'vue';
import MainContainer from 'src/components/MainContainer.vue';
import ContextContainer from 'src/components/ContextContainer.vue';

export default defineComponent({
  components: { MainContainer, ContextContainer },
  name: 'SplitterBoard',
  setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  },
});
</script>
