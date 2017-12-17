<template>
  <div id="app">
    <b-container>
      <b-row>
        <b-col id="heading">
          <h1 class="h1">REINGINEERING.NL</h1>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <terminal></terminal>
        </b-col>
        <b-col>
          <div id="linkedin">
            <iframe src="/static/linkedin.html" allowtransparency="true" frameborder="0" scrolling="0" width="380" height="200"></iframe>
          </div>
          <iframe src="https://ghbtns.com/github-btn.html?user=reinzor&amp;repo=typed.js&amp;type=follow&amp;count=true&amp;size=large" allowtransparency="true" frameborder="0" scrolling="0" width="230" height="50"></iframe>
        </b-col>
      </b-row>
    </b-container>
    <footer class="footer">
      <div class="container">
        <span class="text-muted">COPYRIGHT 2017 - REINGINEERING.NL</span>
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
  background: url(http://cdn.wonderfulengineering.com/wp-content/uploads/2014/04/code-wallpaper-38.jpg) no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  background-size: cover;
  -o-background-size: cover;
  font-family: 'Ubuntu';
}

#heading {
  margin-top: 100px;
  margin-bottom: 50px;
  color: white;
  text-align: center;
}

#linkedin {
  margin-top: -7px;
  margin-left: -7px;
}

.footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  /* Set the fixed height of the footer here */
  height: 60px;
  line-height: 60px; /* Vertically center the text there */
  background-color: rgba(0,0,0,0.5);
}
</style>
