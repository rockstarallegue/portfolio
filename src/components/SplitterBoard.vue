<template>
  <div class="child full container blue-borders rounded-2">
    <q-splitter
      v-model="insideModel"
      separator-class="u-light-glass"
      separator-style="height: 5px"
      class="child full rounded-2 q-pa-xs"
      horizontal
      style="height: 50em;"
    >

      <template v-slot:before>
        <q-splitter
          v-model="splitterModelA"
          separator-class="u-light-glass"
          separator-style="width: 5px"
          class="child full rounded-2"
          style="height: 64em; max-height: 100%"
        >
        <template v-slot:before>
            <div class="full anti-surface rounded-u-l-2 container blue-borders">
              <div class="full child  q-pa-none rounded-u-l-2">
                <MainContainer></MainContainer>
              </div>
            </div>
          </template>

          <template v-slot:separator>
            <q-avatar round color="grey-8" text-color="orange-1" size="sm"
                      icon="grain" class="q-pa-none shadow-1"/>
          </template>

          <template v-slot:after>
            <div class="q-pa-md full container rounded-u-r-2 blue-borders">
              <ContextContainer></ContextContainer>
            </div>
          </template>
        </q-splitter>
      </template>

      <template v-slot:separator>
        <q-avatar round color="grey-8" text-color="orange-1" size="sm"
                  icon="grain" class="q-pa-none shadow-1"/>
      </template>

      <template v-slot:after>
        <q-splitter
          v-model="splitterModelB"
          separator-class="u-light-glass"
          separator-style="width: 5px"
          style="height: 64em; max-height: 100%"
        >
        <template v-slot:before>
            <div class="q-pa-md full container rounded-b-l-2 blue-borders">
              <ContextContainer></ContextContainer>
            </div>
          </template>

          <template v-slot:separator>
            <q-avatar round color="grey-8" text-color="orange-1" size="sm"
                      icon="grain" class="q-pa-none shadow-1"/>
          </template>

          <template v-slot:after>
            <div class="q-pa-md full container rounded-b-r-2 blue-borders">
              <ContextContainer></ContextContainer>
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
