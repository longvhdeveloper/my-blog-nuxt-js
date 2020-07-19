<template>
  <div>
    <Navigation></Navigation>
    <Header :title="title" :sub-title="subTitle"></Header>
    <!-- Main Content -->
    <div class="container">
      <PostList :posts="posts"></PostList>
    </div>
    <hr />
    <Footer></Footer>
  </div>
</template>

<script>
import Navigation from '../components/Navigation'
import Header from '../components/Header'
import Footer from '../components/Footer'
import PostList from '../components/PostList'
export default {
  components: {
    Navigation,
    Header,
    Footer,
    PostList,
  },

  asyncData(ctx) {
    return {
      posts: [
        {
          id: '1',
          title: 'Man must explore, and this is exploration at its greatest',
          subTitle: 'Problems look mighty small from 150 miles up',
          url: '/post?id=1',
          meta: {
            author: 'Mr.Yoda',
            publishDate: '2020-04-10',
          },
        },
        {
          id: '2',
          title:
            "I believe every human has a finite number of heartbeats. I don't intend to waste any of mine.",
          subTitle: '',
          url: '/post?id=2',
          meta: {
            author: 'Mr.Yoda',
            publishDate: '2020-04-12',
          },
        },
        {
          id: '3',
          title: 'Science has not yet mastered prophecy',
          subTitle:
            'We predict too much for the next year and yet far too little for the next ten. ',
          url: '/post?id=3',
          meta: {
            author: 'Mr.Yoda',
            publishDate: '2020-06-15',
          },
        },
        {
          id: '4',
          title: 'Failure is not an option',
          subTitle:
            'Many say exploration is part of our destiny, but it’s actually our duty to future generations. ',
          url: '/post?id=4',
          meta: {
            author: 'Mr.Yoda',
            publishDate: '2020-07-18',
          },
        },
      ],
    }
  },
  data() {
    return {
      posts: {
        type: Array,
      },
      title: "Yoda's Blog",
      subTitle: 'A Blog Theme by Start Bootstrap',
    }
  },
}
</script>
