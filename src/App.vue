<template>
  <div id="app">
  <b-navbar toggleable="md" type="dark">
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <b-navbar-brand href="#">Reingineering</b-navbar-brand>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="mailto:info@reingineering.nl">Email</b-nav-item>
          <b-nav-item href="https://www.linkedin.com/in/rein-appeldoorn-a2b17930">Linkedin</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <b-container>
      <b-row style="margin-top: 20px">
        <b-col style="margin-bottom: 20px">
          <terminal></terminal>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <center>
          <div id="linkedin">
            <iframe src="/static/linkedin.html" allowtransparency="true" frameborder="0" scrolling="0" width="380" height="200"></iframe>
          </div>
          <iframe id="github" src="https://ghbtns.com/github-btn.html?user=reinzor&amp;repo=typed.js&amp;type=follow&amp;count=true&amp;size=large" allowtransparency="true" frameborder="0" scrolling="0" width="230" height="50"></iframe>
          </center>
        </b-col>
      </b-row>
    </b-container>
    <footer class="footer">
      <div class="container">
        <small>copyright 2017-2018 - reingineering.nl</small>
      </div>
    </footer>
  </div>
</template>

<script>
import Terminal from '@/Terminal.vue'

export default {
  name: 'app',
  components: {
    Terminal
  },
  data () {
    return {
    }
  }
}
</script>

<style>
body {
  width: 100wh;
  height: 90vh;
  color: #fff;
  background: linear-gradient(-45deg, #EE7752, #E73C7E, #23A6D5, #23D5AB);
  background-size: 400% 400%;
  -webkit-animation: Gradient 15s ease infinite;
  -moz-animation: Gradient 15s ease infinite;
  animation: Gradient 15s ease infinite;
}

@-webkit-keyframes Gradient {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}

@-moz-keyframes Gradient {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}

@keyframes Gradient {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}

#heading {
  margin-top: 100px;
  margin-bottom: 50px;
  color: white;
  text-align: center;
}

#linkedin {
  margin-top: -7px;
  margin-left: -12px;
}

#github {
  margin-left: -4px;
}

.footer {
  color: white !important;
  position: absolute;
  bottom: 0;
  width: 100%;
  /* Set the fixed height of the footer here */
  height: 60px;
  line-height: 60px; /* Vertically center the text there */
  background-color: rgba(0,0,0,0.5);
}

nav {
  background-color: rgba(0,0,0,0.2) !important;
}
</style>
