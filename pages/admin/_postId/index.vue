<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
  layout: 'admin',
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: 'Maximilian',
        title: 'My awesome Post',
        content: 'Super amazing, thanks for that',
        thumbnailLink: 'https://i8.amplience.net/i/jpl/tech-code-7199c0b6bef7945fd3e7f2467f0fd50d'
      }
    }
  }
}
</script>
