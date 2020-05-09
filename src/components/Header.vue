<template>
  <header class="header">
    <meta property="og:video" content="https://dev-charchalk.pantheonsite.io/wp-content/uploads/2019/12/websitevideoROUGHnoaudio.mp4" />
<meta property="og:video:type" content="video/mp4" />
<meta property="og:video:width" content="1280" />
<meta property="og:video:height" content="720" />
    <b-navbar class="p-0" toggleable="md" type="light">
        <b-navbar-brand>
        <g-link class="logo-home logo-desktop" to="/"><img class="logo-image" alt="logo" src="http://charchalk.imgix.net/03/charchalkblack@2x.png"></g-link>

        <g-link class="logo-home logo–mobile" to="/"><img class="logo-image" alt="logo" src="http://charchalk.imgix.net/03/charchalkblack@2x.png"></g-link>
      </b-navbar-brand>
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav class="ml-auto">
          <g-link class="nav--link" to="/">Shop</g-link>
          <g-link class="nav--link" to="mailto:team@charchalk.com">Contact</g-link>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </header>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style lang="scss">
nav {
  width: 100%;
  padding-top: 1rem;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  background-color: white;
}

.logo-home {
  font-size: 24px;
  max-width: 75%;
  font-weight: bold;
  &:hover {
    text-decoration: none;
  }
}

.logo-desktop {
  @media(max-width: 419px) {
    display: none;
  }
  @media (min-width: 420px) {
    display: default;
  }
}

.logo–mobile {
  @media(max-width: 419px) {
    display: default;
  }
  @media (min-width: 420px) {
    display: none;
  }
}

.logo-image {
  width: 250px;
}

.nav--link {
  margin-left: 20px;
  @media (max-width: 419px) {
    margin: 0;
    padding: 15px 10px 10px 0;
  }
}

.active--exact {
  font-weight: bold;
}
</style>
