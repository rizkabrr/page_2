<template>
  <section class="section">
    <nav class="breadcrumb" aria-label="breadcrumbs">
      <ul>
        <li>
          <a href="#">
            <span class="icon">
              <i class="fas fa-home" aria-hidden="true"></i>
            </span>
            <span>Bulma</span>
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon is-small">
              <i class="fas fa-book" aria-hidden="true"></i>
            </span>
            <span>Documentation</span>
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon is-small">
              <i class="fas fa-puzzle-piece" aria-hidden="true"></i>
            </span>
            <span>Components</span>
          </a>
        </li>
        <li class="is-active">
          <a href="#">
            <span class="icon is-small">
              <i class="fas fa-thumbs-up" aria-hidden="true"></i>
            </span>
            <span>Breadcrumb</span>
          </a>
        </li>
      </ul>
    </nav>
    <!-- -----------------------CONTENT---------------------------- -->

        <div class="card" v-for="(item, i) in items" :key="i">
          <div class="columns">
            <div class="column">
              <figure class="image-figure">
                <img :src="item.image" />
              </figure>
            </div>
            <div class="column">
              <p>Voucher Belanja</p>
              <p class="control" v-if="items.rating">
                <b-rate :value="items.rating" show-score="disabled" />
              </p>
              <hr />
              <b-rate
                v-model="rate"
                :icon-pack="packs"
                :icon="icons"
                :max="maxs"
                :size="sizes"
                :locale="locale"
                :show-score="score"
                :custom-text="custom"
                :show-text="text"
                :texts="texts"
                :rtl="isRtl"
                :spaced="isSpaced"
                :disabled="isDisabled"
              ></b-rate>
            </div>
          </div>
        </div>
  </section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card,
  },

  data() {
    return {
      test: 0,
      items: [
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
      ],
    }
  },
}
</script>
