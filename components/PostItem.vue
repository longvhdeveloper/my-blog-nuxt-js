<template>
  <div class="post-preview">
    <nuxt-link :to="{ name: 'posts-id', params: { id: post.id } }">
      <h2 class="post-title">{{ post.title }}</h2>
      <h3 v-if="post.subTitle" class="post-subtitle">{{ post.subTitle }}</h3>
    </nuxt-link>
    <p class="post-meta">
      Posted by
      <a href="#">{{ post.meta.author }}</a>
      on {{ displayPublishDate }}
    </p>
  </div>
</template>

<script>
import moment from 'moment'
export default {
  props: {
    post: {
      type: Object,
      default() {
        return null
      },
    },
  },
  computed: {
    displayPublishDate() {
      return moment(this.post.meta.publishDate).format('MMMM DD, YYYY')
    },
  },
}
</script>

<style lang="css" scoped>
.post-preview > a {
  color: #212529;
}

.post-preview > a:focus,
.post-preview > a:hover {
  text-decoration: none;
  color: #0085a1;
}

.post-preview > a > .post-title {
  font-size: 30px;
  margin-top: 30px;
  margin-bottom: 10px;
}

.post-preview > a > .post-subtitle {
  font-weight: 300;
  margin: 0 0 10px;
}

.post-preview > .post-meta {
  font-size: 18px;
  font-style: italic;
  margin-top: 0;
  color: #868e96;
}

.post-preview > .post-meta > a {
  text-decoration: none;
  color: #212529;
}

.post-preview > .post-meta > a:focus,
.post-preview > .post-meta > a:hover {
  text-decoration: underline;
  color: #0085a1;
}

@media only screen and (min-width: 768px) {
  .post-preview > a > .post-title {
    font-size: 36px;
  }
}
</style>
