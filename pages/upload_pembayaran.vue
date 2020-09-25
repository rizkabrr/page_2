<template>
  <div class="container">
    <b-field class="title has-text-centered">
      <p><strong>PENDAFTARAN MITRA</strong></p>
    </b-field>
    
    <b-field label="Jenis Jasa" grouped>
      <b-radio v-model="radio" native-value="default">
        Perbaikan/Instalasi
      </b-radio>
      <b-radio v-model="radio" native-value="default">
        Renovasi/Pebangunan
      </b-radio>
      <b-radio v-model="radio" native-value="default">
        Desain
      </b-radio>
      <b-select placeholder="Pilih Jasa" expanded>
        <option value="jenis">Reparasi AC</option>
        <option value="jenis">Reparasi Hitter</option>
      </b-select>
    </b-field>

    <b-field label="Tarif Jasa">
      <div class="table-container has-text-centered">
        <table class="table is-bordered is-striped is-narrow is-hoverable is-fullwidth">
          <thead>
          <tr>
            <th><abbr title="Position">Ketentuan</abbr></th>
            <th><abbr title="Position">Standard</abbr></th>
            <th><abbr title="Position">Medium</abbr></th>
            <th><abbr title="Position">Premium</abbr></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Durasi Pengerjaan</td>
            <td>
              <b-field>
                <b-input></b-input>
              <b-select placeholder="Durasi">
                <option value="dolar">Bulan</option>
                <option value="dolar">Hari</option>
              </b-select>
              </b-field>
            </td>
            <td>
              <b-field>
                <b-input></b-input>
              <b-select placeholder="Durasi">
                <option value="dolar">Bulan</option>
                <option value="dolar">Hari</option>
              </b-select>
              </b-field>
            </td>
            <td>
              <b-field>
                <b-input></b-input>
              <b-select placeholder="Durasi">
                <option value="dolar">Bulan</option>
                <option value="dolar">Hari</option>
              </b-select>
              </b-field>
            </td>
          </tr>
          <tr>
            <td><b-input></b-input></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
          </tr>
          <tr>
            <td><b-input></b-input></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
          </tr>
          <tr>
            <td><b-input></b-input></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
          </tr>
          <tr>
            <td><b-input></b-input></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
            <td><b-checkbox></b-checkbox></td>
          </tr>
        </tbody>
        <tfoot>
          <tr>
            <th><abbr title="Position">Tarif</abbr></th>
            <td>
              <b-select placeholder="Tarif  ">
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
              </b-select>
            </td>
            <td>
              <b-select placeholder="Harga">
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
              </b-select>
            </td>
            <td>
              <b-select placeholder="Harga">
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
                <option value="dolar">$10</option>
              </b-select>
            </td>
          </tr>
        </tfoot>
        </table>
      </div>
    </b-field>

    <b-field title="Cakupan Area">
      <b-select placeholder="Area Cakupan">
        <option value="kota">Kediri</option>
        <option value="kota">Malang</option>
        <option value="kota">Surabaya</option>
      </b-select>
    </b-field>


    <div class="btn has-text-right">
      <b-button position="right">Continue</b-button>
    </div>
  </div>
</template>
<script>
</script>
