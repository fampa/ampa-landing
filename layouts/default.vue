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
                <p class="text-white">
                  Si a la vostra AMPA no teniu ningú capacitat per implementar aquesta app, pode fer-vos un pressupost per implementar-la nosaltres
                </p>
                <br>
                <a class="button is-white is-outlined" href="mailto:jvmonjo@gmail.com" target="_blank">
                  <b-icon
                    icon="email-outline"
                    size="is-small"
                  />
                  <strong>Contacta'ns</strong>
                </a>
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
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column">
              <h3 class="text-white">
                AMPA PWA
              </h3><div class="buttons">
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
            </div>
          </div>
          <p class="text-white">
            Projecte de Final del <strong>Màster de Desenvolupament d'Aplicacions i Llocs Web</strong> de la UOC realitzat per <strong>Josep Vicent Monjo i Agut</strong>.
          </p>
        </div>
      </div>
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
footer {
  font-size: 0.8rem;
}
html {
  background-color: "#1a667e";
}
@media screen and (max-width: 1023px) {
  .navbar-menu {
    background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.3));
  }
}
.text-white, .text-white strong{
  color: white !important;
}

nav.navbar.is-transparent {
    background: transparent;
    color: white;
    width: 100%;
}

nav.navbar.is-transparent a{
    color: white;
}
.heroAlt {
  margin-top: -3.3rem;
  padding-top: 1rem;
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
