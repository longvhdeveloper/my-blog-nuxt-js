<template>
  <div>
    <Navigation></Navigation>
    <Header :title="title" :sub-title="subTitle"></Header>
    <!-- Main Content -->
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-md-10 mx-auto">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe
            nostrum ullam eveniet pariatur voluptates odit, fuga atque ea nobis
            sit soluta odio, adipisci quas excepturi maxime quae totam ducimus
            consectetur?
          </p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eius
            praesentium recusandae illo eaque architecto error, repellendus
            iusto reprehenderit, doloribus, minus sunt. Numquam at quae
            voluptatum in officia voluptas voluptatibus, minus!
          </p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut
            consequuntur magnam, excepturi aliquid ex itaque esse est vero natus
            quae optio aperiam soluta voluptatibus corporis atque iste neque sit
            tempora!
          </p>
        </div>
      </div>
    </div>
    <hr />
    <Footer></Footer>
  </div>
</template>
<script>
import Navigation from '../components/Navigation'
import Header from '../components/Header'
import Footer from '../components/Footer'
export default {
  components: {
    Navigation,
    Header,
    Footer,
  },
  data() {
    return {
      title: 'About me',
      subTitle: 'This is what I do.',
    }
  },
}
</script>
