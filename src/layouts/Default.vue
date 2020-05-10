<template>
  <div class="layout">
    <div id="content-wrapper">
      <Header/>
      <slot/>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from '../components/Footer'
import Header from '../components/Header'

export default {
  components: {
    Footer,
    Header,
  },
}
</script>


<style lang="scss">
body, html {
  height: 100%;
  background-color: #141414;
}

body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Akkurat Mono",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

#app {
  display: flex;
  flex-direction: column;
}

#content-wrapper {
  flex: 1 0 auto;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 20px; 
  padding-right: 20px;
}
</style>
