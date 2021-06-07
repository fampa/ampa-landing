<template>
  <div class="bg-white">
    <section>
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column">
              <h2>Codi obert</h2>
              <p>AMPA PWA és una aplicació de codi obert. Modifica-la com vulguis</p>
              <div class="text-center">
                <img src="@/assets/opensource.png" alt="">
              </div>
            </div>
            <div class="column">
              <h2>Aplicació Web Progressiva (PWA)</h2>
              <p>Es tracta d'una aplicació web que s'adapta a qualsevol mida de pantalla i dispositiu i permet instal·lar-se i rebre notificacions</p>
              <div class="text-center">
                <img src="@/assets/pwa.png" alt="">
              </div>
            </div>
            <div class="column">
              <h2>Gratis!</h2>
              <p>La majoria d'AMPA no requereixen molt recursos per funcionar, i normalment serà suficient usant serveis gratuïts al núvol, però també podeu autoallotjar-la</p>
              <div class="text-center">
                <img src="@/assets/payment.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-grey">
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column">
              <img class="capture is-center" src="@/assets/menu-normal.png" alt="">
              <img class="capture is-center" src="@/assets/menu-admin.png" alt="">
            </div>
            <div class="column is-center">
              <h2>Menú d'administrador</h2>
              <p class="featured">
                Segons els permisos de l'usuari aquest tindrà accés a unes funcions o altres
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column is-center">
              <h2>Gestió de membres</h2>
              <p class="featured">
                Gestiona altes i baixes, enviament de missatges per correu electrònic i notificacions push
              </p>
            </div>
            <div class="column">
              <img class="capture is-center" src="@/assets/envia-missatge.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-grey">
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column">
              <img class="capture is-center" src="@/assets/gestio-contingut.png" alt="">
              <img class="capture is-center" src="@/assets/gestio-contingut-2.png" alt="">
            </div>
            <div class="column is-center">
              <h2>Gestió de continguts</h2>
              <p class="featured">
                Gestiona articles del blog, pàgines, serveis, etiquetes i tot de manera visual i multidioma.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column is-center">
              <h2>Gestió de domiciliacions <br> <span class="dev">en desenvolupament</span> </h2>
              <p class="featured">
                Gestiona les domiciliacions bancàries, la signatura digital del document manament de domiciliacions així com el fitxer de remesa bancària
              </p>
            </div>
            <div class="column">
              <img class="capture is-center" src="@/assets/gestio-remesa.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-grey">
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column">
              <img class="capture is-center" src="@/assets/matriculacio.png" alt="">
            </div>
            <div class="column is-center">
              <h2>Inscripció en serveis</h2>
              <p class="featured">
                Permet matricular en serveis amb un sol click, gestiona la capacitat del servei, el llistat de matriculats i notifica automàticament per correu electrònic.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <div class="content">
          <div class="columns">
            <div class="column">
              <h2>Tutorials</h2>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <div class="video-responsive">
                <iframe
                  src="https://www.youtube.com/embed/13Kgsa1OURY"
                  title="YouTube video player"
                  frameborder="0"
                  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                  allowfullscreen
                />
              </div>
            </div>
            <div class="column">
              <div class="video-responsive">
                <iframe
                  src="https://www.youtube.com/embed/QaIEomSMjLs"
                  title="YouTube video player"
                  frameborder="0"
                  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                  allowfullscreen
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>

export default {
  name: 'HomePage'
}
</script>

<style>
.video-responsive {
  height: 0;
  overflow: hidden;
  padding-bottom: 56.25%;
  padding-top: 30px;
  position: relative;
}
.video-responsive iframe, .video-responsive object, .video-responsive embed {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
.dev {
  opacity: 0.8;
  font-size: 0.8rem;
  text-transform: uppercase;
}
.bg-white {
  background-color: white;
}
.bg-grey {
  background-color: rgb(243, 243, 243);
}
.featured {
  font-size: 1.8rem;
}
.text-right {
  text-align: right;
}
.capture {
  max-height: 400px;
  max-width: 45%;
}
.has-bg-img {
  background: url('/assets/images/img.jpg')center center;
  background-size:cover;
}
.text-center {
  text-align: center;
}
.container {
  padding: 2rem;
}
</style>
