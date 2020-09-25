<template>
  <div class="container">
    <b-field class="title has-text-centered">
      <p><strong>PROFIL MITRA</strong></p>
    </b-field>

    <div class="card px-2 py-2 mt-2 mb-6">
      <div class="columns is-mobile is-multiline">
      <div class="column is-one-fifth">
        <p>Nama Jasa</p>
      </div>
      <div class="column">
        <p><span> : </span>Nama Jasa</p>
      </div>
    </div>

    <div class="columns is-mobile is-multiline">
      <div class="column is-one-fifth">
        <p>Pemilik Jasa</p>
      </div>
      <div class="column">
        <p><span> : </span>Nama Jasa</p>
      </div>
    </div>

    <div class="columns is-mobile is-multiline">
      <div class="column kategori is-one-fifth">
        <p>Kategori</p>
      </div>
      <div class="column">
        <p><span>:</span> Pembangunan/Renovasi</p>
      </div>
    </div>

    <div class="columns is-mobile is-multiline">
      <b-field class="column is-one-fifth">
        <b-icon icon="map"></b-icon>
        <p>Area Cakupan</p>
      </b-field>
      <div class="column">
        <span> : </span>
        <b-tag>Kediri</b-tag>
        <b-tag>Blitar</b-tag>
        <b-tag>Tulungagung</b-tag>
      </div>
    </div>

    <div class="columns is-mobile is-multiline">
      <div class="column kategori is-one-fifth">
        <p>Deskripsi</p>
      </div>
      <div class="column">
        <p><span>: </span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde tempora, ducimus distinctio nihil sed et provident aperiam sequi omnis vel eius ratione quaerat, perspiciatis quam? Natus magnam accusantium aliquam id.</p>
      </div>
    </div>
    </div>

    <b-field class="card has-text-centered">
      <div class="columns is-mobile is-multiline">
        <div class="column is-one-third">
          <img src="~assets/2.png" alt="">
        </div>
        <div class="column is-one-third">
          <img src="~assets/2.png" alt="">
        </div>
        <div class="column is-one-third">
          <img src="~assets/2.png" alt="">
        </div>
        <div class="column is-one-third">
          <img src="~assets/2.png" alt="">
        </div>
        <div class="column is-one-third">
          <img src="~assets/2.png" alt="">
        </div>
        <div class="column is-one-third">
          <img src="~assets/2.png" alt="">
        </div>
      </div>
    </b-field>

    <b-field label="Tarif Jasa">
      <div class="table-container has-text-centered">
        <table
          class="table is-bordered is-striped is-narrow is-hoverable is-fullwidth"
        >
          <thead>
            <tr>
              <th><abbr title="Position">Ketentuan</abbr></th>
              <th><abbr title="Position">Standard</abbr></th>
              <th><abbr title="Position">Medium</abbr></th>
              <th><abbr title="Position">Premium</abbr></th>
            </tr>
          </thead>
          <tbody>
            <tr class="text has-text-left">
              <td class="text has-text-centered">Deskripsi Harga</td>
              <td><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste unde omnis nesciunt autem assumenda laboriosam porro aliquid fuga illo pariatur incidunt, in, explicabo nobis quia, tenetur fugiat? Aperiam, numquam corrupti?</p></td>
              <td><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste unde omnis nesciunt autem assumenda laboriosam porro aliquid fuga illo pariatur incidunt, in, explicabo nobis quia, tenetur fugiat? Aperiam, numquam corrupti?</p></td>
              <td><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste unde omnis nesciunt autem assumenda laboriosam porro aliquid fuga illo pariatur incidunt, in, explicabo nobis quia, tenetur fugiat? Aperiam, numquam corrupti?</p></td>
            </tr>
            <tr>
              <td>Durasi Pengerjaan</td>
              <td>
                <b-field class="durasi">
                  <p>3<span>-</span>Bulan</p>
                </b-field>
              </td>
              <td>
                <b-field class="durasi">
                  <p>2<span>-</span>Bulan</p>
                </b-field>
              </td>
              <td>
                <b-field class="durasi">
                  <p>1<span>-</span>Bulan</p>
                </b-field>
              </td>
            </tr>
            <tr>
              <td>Babibaba</td>
              <td><b-icon icon="check"></b-icon></td>
              <td><b-icon icon="check"></b-icon></td>
              <td><b-icon icon="check"></b-icon></td>
            </tr>
            <tr>
              <td>Babakebab</td>
              <td><b-icon icon="check"></b-icon></td>
              <td><b-icon icon="check"></b-icon></td>
              <td><b-icon icon="check"></b-icon></td>
            </tr>
            <tr>
              <td>Berakberak</td>
              <td><b-icon icon="strip"></b-icon></td>
              <td><b-icon icon="check"></b-icon></td>
              <td><b-icon icon="check"></b-icon></td>
            </tr>
            <tr>
              <td>Cerurutan</td>
              <td></td>
              <td></td>
              <td><b-icon icon="check"></b-icon></td>
            </tr>
          </tbody>
          <tfoot>
            <tr>
              <th><abbr title="Position">Tarif</abbr></th>
              <td><strong>$30</strong></td>
              <td><strong>$40</strong></td>
              <td><strong>$50</strong></td>
            </tr>
          </tfoot>
        </table>
      </div>
    </b-field>

    <div class="btn has-text-right">
      <b-button position="right">Continue</b-button>
    </div>
  </div>
</template>
<script></script>
<style>
.field.durasi {
    font-size: x-large;
}
/* .column {
    background-color:aquamarine;
    border-width: thin;
} */
</style>
