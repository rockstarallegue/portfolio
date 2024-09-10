<template>
  <div class="child full rounded-u-l-2 blue-borders light-glass container">
   <div class="full row rounded-u-l-2 blue-borders">
    <div class="child full col-6 q-pa-none container">
      <!-- COMMITTERS BOX -->
      <div class="child full col-5 rounded-2 container">
        <NodeBox></NodeBox>
      </div>
    </div>
    <q-separator vertical color="blue-grey-3"/>
    <div class="child full col q-pa-none container">
      <div class="child full column rounded-2">
        <!-- COMMITTERS BOX -->
        <div class="child full col-5 rounded-2 container">
          <CommittersBox></CommittersBox>
        </div>
        <q-separator horizontal color="blue-grey-3"/>
        <!-- COMMITTERS BOX -->
        <div class="child full col-6 rounded-2 container">
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
