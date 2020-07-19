<template>
  <!-- Footer -->
  <footer>
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-md-10 mx-auto">
          <ul class="list-inline text-center">
            <li class="list-inline-item">
              <nuxt-link to="#">
                <span class="fa-stack fa-lg">
                  <i class="fas fa-circle fa-stack-2x"></i>
                  <i class="fab fa-twitter fa-stack-1x fa-inverse"></i>
                </span>
              </nuxt-link>
            </li>
            <li class="list-inline-item">
              <nuxt-link to="#">
                <span class="fa-stack fa-lg">
                  <i class="fas fa-circle fa-stack-2x"></i>
                  <i class="fab fa-facebook-f fa-stack-1x fa-inverse"></i>
                </span>
              </nuxt-link>
            </li>
            <li class="list-inline-item">
              <nuxt-link to="#">
                <span class="fa-stack fa-lg">
                  <i class="fas fa-circle fa-stack-2x"></i>
                  <i class="fab fa-github fa-stack-1x fa-inverse"></i>
                </span>
              </nuxt-link>
            </li>
          </ul>
          <p class="copyright text-muted">
            Copyright &copy; Yoda Blog Website {{ currentYear }}
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      currentYear: new Date().getFullYear(),
    }
  },
}
</script>

<style lang="css" scoped>
footer {
  padding: 50px 0 65px;
}

footer .list-inline {
  margin: 0;
  padding: 0;
}

footer .copyright {
  font-size: 14px;
  margin-bottom: 0;
  text-align: center;
}
</style>
