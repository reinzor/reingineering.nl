<template>
  <div id="app">
    <div class="header">
      <div class="head-wrap shift-text">
        <h1 class="h1">REINGINEERING.NL</h1>
        <div class="text-editor-wrap">
          <div class="title-bar"><span class="title">bash — 80x<span class="terminal-height">20</span></span></div>
          <div class="text-body">
            <vue-typer :text='introText'></vue-typer>
          </div>
        </div>
      </div>
      <div class="wrap">
        <div class="btn-wrap">
          <iframe src="https://ghbtns.com/github-btn.html?user=reinzor&amp;repo=typed.js&amp;type=follow&amp;count=true&amp;size=large" allowtransparency="true" frameborder="0" scrolling="0" width="300" height="50"></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { VueTyper } from 'vue-typer'

export default {
  name: 'app',
  components: {
    VueTyper
  },
  data () {
    return {
      introText: `Welcome to my website ..

Hi there!
`
    }
  }
}
</script>

<style>
html {
  background: url(http://cdn.wonderfulengineering.com/wp-content/uploads/2014/04/code-wallpaper-38.jpg) no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}

#app {
  font-family: 'Ubuntu';
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.header {
  width: 100%;
  height: 100%;
  margin: 0 auto 30px;
  padding: 10px 0;
}

.header .h1 {
  margin: 10px 0 20px;
  font-size: 2.5em;
  text-align: center;
  color: #fff;
  text-shadow: #000 0px 2px 4px; }

.head-wrap {
  margin: 30px auto 30px;
  -webkit-transition: all 0.5s ease-out;
  -moz-transition: all 0.5s ease-out;
  -ms-transition: all 0.5s ease-out;
  -o-transition: all 0.5s ease-out;
  transition: all 0.5s ease-out;
  text-align: center;
}

/* text editor styles */
.text-editor-wrap {
  display: block;
  margin: auto;
  max-width: 530px;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.8) 0px 20px 70px;
  clear: both;
  overflow: hidden;
  -webkit-transition: all 0.5s ease-out;
  -moz-transition: all 0.5s ease-out;
  -ms-transition: all 0.5s ease-out;
  -o-transition: all 0.5s ease-out;
  transition: all 0.5s ease-out;
}

.text-editor-wrap .custom.char {
  color: white;
}

.title-bar {
  padding: 5px 0;
  font-family: "Lucida Grande", sans-serif;
  font-size: 0.75em;
  text-align: center;
  text-shadow: rgba(255, 255, 255, 0.8) 0px 1px 0px;
  background-color: #f8f8f8;
  background-image: -webkit-linear-gradient(top, #e8e8e8, #bcbbbc);
  background-image: -moz-linear-gradient(top, #e8e8e8, #bcbbbc);
  background-image: linear-gradient(top, #e8e8e8, #bcbbbc);
  box-shadow: inset rgba(255, 255, 255, 0.7) 0px 1px 1px;
  border-bottom: #6a6a6a 1px solid;
}

.text-body {
  height: 250px;
  background-color: rgba(0, 0, 0, 0.85);
  padding: 10px;
  color: #f0f0f0;
  text-shadow: #000 0px 1px 0px;
  font-family: "Consolas", "Courier New", "Courier";
  font-size: 1.45em;
  line-height: 1.40em;
  font-weight: 500;
  text-align: left;
  overflow: hidden;
  -webkit-transition: all 0.5s ease-out;
  -moz-transition: all 0.5s ease-out;
  -ms-transition: all 0.5s ease-out;
  -o-transition: all 0.5s ease-out;
  transition: all 0.5s ease-out;
}

</style>
