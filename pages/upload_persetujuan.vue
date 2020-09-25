<template>
  <div class="container">
    <b-field class="title has-text-centered">
      <p><strong>PENDAFTARAN MITRA</strong></p>
    </b-field>

    <b-field label="Nama Penanggung Jawab">
      <b-input></b-input>
    </b-field>

    <b-field label="No Telp Penanggung Jawab">
      <b-input></b-input>
    </b-field>

    <b-field label="Alamat Penggung Jawab">
      <div class="columns is-mobile">
        <div class="column is-2">
          <b-select placeholder="Negara" expanded>
            <option value="negara">Indonesia</option>
          </b-select>
        </div>
        <div class="column is-2">
          <b-select placeholder="Provinsi" expanded>
            <option value="Provinsi">Jawa Timur</option>
          </b-select>
        </div>
        <div class="column is-2">
          <b-select placeholder="Kabupaten/Kota" expanded>
            <option value="Kabupaten/Kota">Kediri</option>
          </b-select>
        </div>
      <div class="column">
        <b-input expanded>
          <option value="Keterangan"></option>
        </b-input>
      </div>
      </div>
    </b-field>

    <b-field label="Upload KTP" group>
      <b-upload v-model="dropFiles" multiple drag-drop expanded>
        <section class="section">
          <div class="content has-text-centered">
            <p>
              <b-icon icon="upload" size="is-large"> </b-icon>
            </p>
            <p>Drop your files here or click to upload</p>
          </div>
        </section>
      </b-upload>
    </b-field>

    <div class="tags">
      <span
        v-for="(file, index) in dropFiles"
        :key="index"
        class="tag is-primary"
      >
        {{ file.name }}
        <button
          class="delete is-small"
          type="button"
          @click="deleteDropFile(index)"
        ></button>
      </span>
    </div>

    <b-field>
      <b-toast class="message has-text-centerd">
        Maksimal File 10Mb, diharapkan file KTP memiliki kualitas yang baik dan
        jelas
      </b-toast>
    </b-field>

    <b-field label="Upload NPWP (jika memiliki)" group>
      <b-upload v-model="dropFiles" multiple drag-drop expanded>
        <section class="section">
          <div class="content has-text-centered">
            <p>
              <b-icon icon="upload" size="is-large"> </b-icon>
            </p>
            <p>Drop your files here or click to upload</p>
          </div>
        </section>
      </b-upload>
    </b-field>
    <div class="tags">
      <span
        v-for="(file, index) in dropFiles"
        :key="index"
        class="tag is-primary"
      >
        {{ file.name }}
        <button
          class="delete is-small"
          type="button"
          @click="deleteDropFile(index)"
        ></button>
      </span>
    </div>

    <b-field>
      <b-toast class="message has-text-centerd">
        Maksimal File 10Mb, diharapkan file NPWP memiliki kualitas yang baik dan
        jelas
      </b-toast>
    </b-field>

    <b-field grouped class="cek pt-3">
      <b-checkbox size="is-medium"
        >Saya akan mematuhi kebijakan yang berlaku</b-checkbox
      >
    </b-field>

    <b-field>
      <b-input type="textarea"></b-input>
    </b-field>

    <b-field>
      <b-button position="right">Upload</b-button>
    </b-field>
  </div>
</template>
<script>
export default {
  data() {
    return {
      dropFiles: [],
    }
  },
  methods: {
    deleteDropFile(index) {
      this.dropFiles.splice(index, 1)
    },
  },
}
</script>
