<template>
  <header class="header">
    <meta property="og:video" content="https://dev-charchalk.pantheonsite.io/wp-content/uploads/2019/12/websitevideoROUGHnoaudio.mp4" />
<meta property="og:video:type" content="video/mp4" />
<meta property="og:video:width" content="1280" />
<meta property="og:video:height" content="720" />

       
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
}

a.btn.btn-primary {
    font-size: 20px;
    text-transform: uppercase;
    background-clip: border-box;
    border-top-width: 3px;
    border-right-width: 3px;
    border-bottom-width: 3px;
    border-left-width: 3px;
    border-top-left-radius: 35px;
    border-top-right-radius: 35px;
    border-bottom-left-radius: 35px;
    border-bottom-right-radius: 35px;
}

.nav--link {
           font-family: "Akkurat Mono";
    font-size: 25px !important;
    color: white;
    text-transform: uppercase;
    &:hover {
      text-decoration: none;
    }
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
    text-align: center;
     display: flex;
    align-items: center;
    justify-content: center;
  }
  @media (min-width: 420px) {
    display: none;
  }
}


.logo-image {
    width: 250px;
    padding-left: 5px;
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
