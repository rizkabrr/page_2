<template>
  <section class="section">
    <div class="columns is-multiline is-mobile is-variable">
      <div class="column is-one-third" v-for="(item, i) in items" :key="i">
        <div class="card">
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
      </div>
    </div>
   <div>
     <button class="button is-small is-fullwidth">Small</button>
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
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://cdna.artstation.com/p/assets/images/images/010/098/130/large/sajal-kr-chand-flat-landscape.jpg?1522574693',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/7db5c985847371.5d8898692240d.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/49e7f485847371.5d8898692146c.jpg',
          rating: 5,
        },
      ],
    }
  },
}
</script>
