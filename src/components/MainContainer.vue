<template>
  <div class="child full bg-blue-grey-8 rounded-2 container">
   <div class="full row rounded-2 blue-borders">
    <div class="child full col-6 q-py-sm q-pl-sm q-pr-sm container">
      <!-- COMMITTERS BOX -->
      <div class="child full col-5 rounded-2 shadow-1 container">
        <NodeBox></NodeBox>
      </div>
    </div>
    <div class="child full col q-py-sm q-pl-xs q-pr-sm container">
      <div class="child full column rounded-2">
        <!-- COMMITTERS BOX -->
        <div class="child full col-5 rounded-2 shadow-1 container">
          <CommittersBox></CommittersBox>
        </div>
        <!-- AESTHETIC SPACE -->
        <div class="child full col"></div>
        <!-- COMMITTERS BOX -->
        <div class="child full col-6 rounded-2 shadow-1 container">
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
