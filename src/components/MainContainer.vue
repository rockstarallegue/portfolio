<template>
  <div class="child full rounded-u-l-2 container">
   <div class="full row rounded-u-l-2 blue-borders light-glass">
    <div class="child full col-5 q-pa-none container">
      <!-- COMMITTERS BOX -->
      <div class="child full col-5 rounded-2 container">
        <NodeBox></NodeBox>
      </div>
    </div>
    <q-separator vertical color="grey-5" />
    <div class="child full col q-pa-none q-pt-xs container">
      <div class="child full column container">
        <!-- COMMITTERS BOX -->
        <div class="child col-5 container">
          <CommittersBox></CommittersBox>
        </div>
        <q-separator horizontal color="grey-5"/>
        <!-- COMMITTERS BOX -->
        <div class="child full col-5 container">
          <TagsBox></TagsBox>
        </div>
      </div>
    </div>
   </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import CommittersBox from 'src/components/Boxes/CommittersBox.vue';
import TagsBox from 'src/components/Boxes/TagsBox.vue';
import NodeBox from 'src/components/Boxes/NodeBox.vue';

export default defineComponent({
  components: { CommittersBox, TagsBox, NodeBox },
  name: 'MainContainer',
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
