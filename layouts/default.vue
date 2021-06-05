<template>
  <div>
    <header>
      <b-navbar :transparent="true">
        <template #brand>
          <b-navbar-item class="site-title" tag="router-link" :to="{ path: '/' }">
            AMPA PWA
          </b-navbar-item>
        </template>
        <template #start>
          <b-navbar-item v-for="(item, index) in items" :key="index" tag="router-link" :to="item.to">
            {{ item.title }}
          </b-navbar-item>
          <b-navbar-item v-for="(item, index) in external" :key="index" :href="item.href">
            {{ item.title }}
          </b-navbar-item>
        </template>

        <template #end>
          <b-navbar-item tag="div">
            <div class="buttons">
              <a class="button is-primary" style="color:white; background:#0f3946;" href="https://github.com/fampa/ampa-pwa" target="_blank">
                <b-icon
                  icon="github"
                  size="is-small"
                />
                <strong>Github</strong>
              </a>
              <a class="button is-white is-outlined" href="https://fampa-pwa.web.app" target="_blank">
                <b-icon
                  icon="cellphone-text"
                  size="is-small"
                />
                <strong>App d'exemple</strong>
              </a>
            </div>
          </b-navbar-item>
        </template>
      </b-navbar>
      <section class="heroAlt">
        <div class="container">
          <div class="hero-body">
            <div class="columns">
              <div class="column is-center">
                <p class="title text-white">
                  Gestiona la teva AMPA online
                </p>
                <p class="subtitle text-white">
                  Una app de codi obert a l'abast de tothom
                </p>
              </div>
              <div class="column is-bottom">
                <img src="@/assets/mum.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </section>
    </header>
    <main>
      <Nuxt />
    </main>
    <footer>
      footer
    </footer>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        // {
        //   title: 'Inici',
        //   icon: 'home',
        //   to: { path: '/' }
        // }
      ],
      external: [
        // {
        //   title: 'Documentació',
        //   href: 'https://github.com/fampa/ampa-pwa'
        // }
      ]
    }
  }
}
</script>

<style>
.text-white{
  color: white !important;
}
nav.navbar.is-transparent {
    background: transparent;
    color: white;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
}

nav.navbar.is-transparent a{
    color: white;
}
.heroAlt {
  background: linear-gradient(rgba(26, 102, 126, 1), rgba(26, 102, 126, 1),rgba(26, 102, 126, 0.9), rgba(26, 102, 126, 0.6));
}
a.navbar-burger.burger {
    color: white;
}
.site-title {
  font-weight: 700;
}
.is-bottom {
  align-self: flex-end;
}

.is-center {
  align-self: center;
}
</style>
