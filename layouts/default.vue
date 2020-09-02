<template>
  <!-- <section class="container"> -->
    <div>
      <nav
        class="navbar header has-shadow is-fluid"
        role="navigation"
        aria-label="main navigation"
      >
        <div class="navbar-brand">
          <a class="navbar-item" href="#">
            <img src="~/assets/2.png" width="150" />
          </a>

          <a
            role="button"
            class="navbar-burger burger"
            aria-label="menu"
            aria-expanded="false"
            data-target="navbarBasicExample"
          >
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div class="navbar-start">
          <b-field class="py-2 pl-4">
            <b-input
              placeholder="Pencarian..."
              type="search"
              icon-right="magnify"
              icon-right-clickable="search"
            />
          </b-field>
        </div>
        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <a class="button is-light">
                <strong>Gabung Mitra</strong>
              </a>
              <a class="button is-halo">
                <strong>Masuk</strong>
              </a>
            </div>
          </div>
        </div>
      </nav>
      <div class="container">
      <div>
        <nav class="breadcrumb has-arrow-separator" aria-label="breadcrumbs">
          <ul>
            <li>
              <a href="#">Bulma</a>
            </li>
            <li>
              <a href="#">Documentation</a>
            </li>
            <li>
              <a href="#">Components</a>
            </li>
            <li class="is-active">
              <a href="#" aria-current="page">Breadcrumb</a>
            </li>
          </ul>
        </nav>
      </div>

      <section class="main-content columns">
        <aside class="column is-2 section px-4">
          <p class="menu-label is-hidden-touch">General</p>
          <ul class="menu-list">
            <li v-for="(item, key) of items" :key="key">
              <nuxt-link :to="item.to" exact-active-class="is-active">
                <b-icon :icon="item.icon" />
                {{ item.title }}
              </nuxt-link>
            </li>
          </ul>

          <div>
            <b>Kategori</b>
            <p>----------------</p>
            <div class="field">
              <b-checkbox>Konsep Desain Rumah</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Konsep Desain Gedung</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Konsep Desain Taman</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Konsep Desain Ruangan</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Others</b-checkbox>
            </div>
          </div>

          <b-field label="Biaya">
            <b-slider :value="20"></b-slider>
          </b-field>

          <div>
            <b>Level Mitra</b>
            <p>----------------</p>
            <div class="field">
              <b-checkbox>Mitra Baru</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Mitra Level 1</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Mitra Level 2</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Top Mitra</b-checkbox>
            </div>
          </div>

          <div>
            <b>Tampilan Projek</b>
            <p>----------------</p>
            <div class="field">
              <b-checkbox>3D</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Sket Pensil</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Mapping</b-checkbox>
            </div>
            <div class="field">
              <b-checkbox>Others</b-checkbox>
            </div>
          </div>
        </aside>

        <div class="container column is-10">
          <nuxt />
        </div>
      </section>
      </div>
      <div>
        <footer class="footer">
          <div class="content">
            <div class="columns">
              <div class="column">
                <h1>Halo Properti</h1>
                <div class="columns">
                    <a class="icon-f" href="#">
                      <img src="https://img.icons8.com/material-rounded/24/000000/facebook-new.png"/>
                    </a>
                    <a class="icon-f" href="#">
                      <img src="https://img.icons8.com/material-rounded/24/000000/youtube.png"/>
                    </a>
                    <a class="icon-f" href="#">
                      <img src="https://img.icons8.com/material-rounded/24/000000/pinterest.png"/>
                    </a>
                    <a class="icon-f" href="#">
                      <img src="https://img.icons8.com/material-rounded/24/000000/instagram-new.png"/>
                    </a>
                </div>
              </div>
              <div class="column">
                <div class="columns">
                  <br/>
                </div>
                <div>
                  <a href="#">
                    <h3>Tentang Kami</h3>
                  </a>
                </div>
                <div>
                  <a href="#">
                    <h3>Layanan Kami</h3>
                  </a>
                </div>
                <div>
                  <a href="#">
                    <h3>Kebijakan Kami</h3>
                  </a>
                </div>
                <div>
                  <a href="#">
                    <h3>Kebijakan Peivasi</h3>
                  </a>
                </div>
              </div>
              <div class="column">
                <div class="columns">
                  <br/>
                </div>
                <div >
                  <a href="#">
                    <h3>Patner Kami</h3>
                  </a>
                </div>
                <div>
                  <a href="#">
                    <h3>Kontak Kami</h3>
                  </a>
                </div>
                <div>
                  <a href="#">
                    <h3>Pusat Bantuan</h3>
                  </a>
                </div>
                <div>
                  <a href="#">
                    <h3>Kebijakan Privasi</h3>
                  </a>
                </div>
              </div>
              <div class="column">
                <div class="columns">
                  <br/>
                </div>
                <div class="column">
                <div class="columns">
                  <h3>Unduh Aplikasi</h3>
                </div>
                <div class="columns">
                  <a class="a1" href="#">
                    <img src="~assets/icon_gp.png" alt="play_store" />
                  </a>
                  <a class="a1" href="#">
                    <img src="~assets/icon_as.png" alt="app_store" />
                  </a>
                </div>
                <div>
                  <h3>Ikuti Kami</h3>
                </div>
                </div>
              </div>
            </div>
          </div>
        </footer>
      </div>
    </div>
  <!-- </section> -->
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' },
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' },
        },
      ],
    }
  },
}
</script>
<style>
.navbar.is-primary {
  background-color: white;
}
.b-gabung {
  color: aqua;
}
.footer {
  background-color: #f6924b;
  padding: 3rem 1.5rem 6rem;
}
.b-slider.is-primary .b-slider-fill {
  background: #f79651 !important;
}
.button.is-light {
  background-color: #f79651;
  border-color: transparent;
  /* color: rgba(0, 0, 0, 0.7); */
  color: white;
}
.menu-list a.is-active {
  background-color: #f79651;
  color: #fff;
}
.menu-list a:hover {
  background-color: #f7965126;
  color: #363636;
}
.section {
    padding: 1rem 1rem;
}
article, aside, figure, footer, header, hgroup, section {
    display: grid;
}
body{
  font-size: small;
}
.icon-f{
  padding: 10px;
}
.a1{
  width: 240px;
  height: auto; 
}
</style>