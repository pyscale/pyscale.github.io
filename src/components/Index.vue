<template>
  <b-container fluid>
    <b-nav tabs>
      <b-nav-item href="#" style="color: #274C77;">
        <b-link href="#">Home</b-link>
      </b-nav-item>
      <b-nav-item-dropdown text="Services" right style="color: #274C77;">
        <b-dropdown-item>
          <b-link href="#ml" style="color: #274C77;">Machine Learning</b-link>
        </b-dropdown-item>
        <b-dropdown-item>
          <b-link href="#big-data" style="color: #274C77;">Big Data</b-link>
        </b-dropdown-item>
      </b-nav-item-dropdown>
      <b-nav-item-dropdown text="Products" right style="color: #274C77;">
        <b-dropdown-item>
          <b-link href="https://curate.pyscale.net" style="color: #274C77;">Landing Page Curation</b-link>
        </b-dropdown-item>
        <b-dropdown-item>
          <b-link href="#" style="color: #274C77;" disabled>Authenic Artist</b-link>
        </b-dropdown-item>
      </b-nav-item-dropdown>
    </b-nav>

    <b-container fluid style="background-color: #274C77">
      <b-jumbotron id='#' style="background-color: #274C77; color: white">
        <h2 class="display-4">PyScale, LLC</h2>
        <p class="lead">Building Scalable Pythonic Solutions</p>
        <hr class="my-4">
        <p class="lead">Go Beyond Your Limits</p>
      </b-jumbotron>
    </b-container>
    <b-container fluid>
      <b-card id="#services" class="border-light">
        <b-card-body style="background-color: white">
          <b-jumbotron style="color: #274C77; background-color: white">
            <h2 class="display-4">Current Service Offerings</h2>
            <p>
                Here at <strong>PyScale, LLC</strong>, our focus is that your business
                project requirements are met, and actionable insights are gathered
                to support the velocity of your team.

                Please consider the below material to understand which of your needs
                are best satisfied below.

                Additionally, we are certified to construct your cloud infrastructure within AWS.

                We have full confidence to manage your AWS solution architecture given our
                <a href="https://www.youracclaim.com/badges/85002cbf-f65d-4a14-9534-030cccfd3ae0">certification</a>

                For any inquires, please consult the form below.
            </p>
          </b-jumbotron>
        </b-card-body>
        <b-card-footer class="bg-transparent">
          <b-card-group>
            <b-card id="#ml" class="border-light">
              <b-card-title>
                Machine Learning
              </b-card-title>
              <b-card-body>
                <b-card-text>
                  <strong>The rise of the machine</strong> has given mankind the ability to generate applications
                  to provide value.  Do you want to recommend products?  Do you want to predict the value of
                  residential properties?
                </b-card-text>
              </b-card-body>
            </b-card>
            <b-card id="#big-data" class="border-light">
              <b-card-title>
                Big Data
              </b-card-title>
              <b-card-body>
                <b-card-text>
                  Given the efficiency of collecting information to better serve consumers, the traditional
                  methods to extract, transform and load data has slowly became ineffective.  We are now at the
                  cusp of change.  Are you at that point?  Are you constantly receiving Memory Overflow errors when
                  processing large volumes of data? Does it take days to process your data using
                  traditional processes?
                </b-card-text>
              </b-card-body>
            </b-card>
          </b-card-group>
        </b-card-footer>
      </b-card>
    </b-container>
    <footer>
      <p>
          For all inquires, please fill out this the following
          <b-link v-b-modal.modal-1>form</b-link>
      </p>
      <p>
      Social:

      <a href="https://twitter.com/PyScaleLLC?ref_src=twsrc%5Etfw" class="twitter-follow-button" data-show-count="false">Follow @PyScaleLLC</a><script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

      </p>
      <b-modal id="modal-1" size="xl" hide-header hide-footer>
        <b-embed
        type="iframe"
        aspect="16by9"
        src="https://docs.google.com/forms/d/e/1FAIpQLSdIuOUZqXWhMbCmRnITTP9pecADl49OdYoAGLaSf3ZicuDcUg/viewform?embedded=true"
        >
        </b-embed>
      </b-modal>

    </footer>
  </b-container>
</template>

<script>
import Vue from 'vue'
import { LinkPlugin, ModalPlugin, LayoutPlugin, CardPlugin, JumbotronPlugin, EmbedPlugin, NavPlugin, NavbarPlugin, DropdownPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

Vue.use(LinkPlugin)
Vue.use(ModalPlugin)
Vue.use(LayoutPlugin)
Vue.use(CardPlugin)
Vue.use(JumbotronPlugin)
Vue.use(NavbarPlugin)
Vue.use(NavPlugin)
Vue.use(DropdownPlugin)
Vue.use(EmbedPlugin)

export default {
  name: 'Index'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
