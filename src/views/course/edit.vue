<template>
  <div class="course-list">
    <create-or-update is-edit :course-id="courseId" />
  </div>
</template>

<script lang="ts">
  import Vue from 'vue'
  import CreateOrUpdate from './components/CreateOrUpdate.vue'

  export default Vue.extend({
    name: 'CourseEditor',
    props: {
      courseId: {
        type: [String, Number],
        required: true
      }
    },
    components: {
      CreateOrUpdate
    }
  })
</script>

<style lang="scss" scoped>
</style>
