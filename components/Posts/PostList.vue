<template>
    <section class="post-list">
      <PostPreview
        id="1"
        :is-admin="isAdmin"
        thumbnail="https://i8.amplience.net/i/jpl/tech-code-7199c0b6bef7945fd3e7f2467f0fd50d"
        title="Hello there"
        previewText="This my first post"
        />
      <PostPreview
        id="2"
        :is-admin="isAdmin"
        thumbnail="https://i8.amplience.net/i/jpl/tech-code-7199c0b6bef7945fd3e7f2467f0fd50d"
        title="Hello there - the second time"
        previewText="This my second post!"
        />
      <PostPreview
        id="3"
        :is-admin="isAdmin"
        thumbnail="https://i8.amplience.net/i/jpl/tech-code-7199c0b6bef7945fd3e7f2467f0fd50d"
        title="Hi"
        previewText="This my third post!"
        />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>
