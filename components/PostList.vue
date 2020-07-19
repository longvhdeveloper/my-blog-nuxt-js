<template>
  <div class="row">
    <div class="col-lg-8 col-md-10 mx-auto">
      <PostItem v-for="post in posts" :key="post.id" :post="post"></PostItem>
      <hr />
      <Pager></Pager>
    </div>
  </div>
</template>

<script>
import PostItem from '../components/PostItem'
import Pager from '../components/Pager'
export default {
  components: {
    PostItem,
    Pager,
  },
  props: {
    posts: {
      type: Array,
      default() {
        return []
      },
    },
  },
  data() {
    return {
      postList: {
        type: Array,
        default: [],
      },
    }
  },
}
</script>
