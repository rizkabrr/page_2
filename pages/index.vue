<template>
  <section class="section">
    <div class="columns is-multiline is-mobile is-variable">
      <div class="column is-one-third" v-for="(item, i) in items" :key="i">
        <!-- <div class="card"> -->
        <div class="columns">
          <div class="column">
            <div class="image IMG-F">
              <figure class="image-figure">
                <img :src="item.image" />
              </figure>
            </div>
          </div>
          <!-- <div class="column">
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
            </div> -->
        </div>
        <!-- </div> -->
      </div>
    </div>
    <div class="see-more">
      <button class="button is-fullwidth"><strong>Small</strong></button>
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
            'https://upload.wikimedia.org/wikipedia/commons/f/f5/Poster-sized_portrait_of_Barack_Obama.jpg',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image:
            'https://images.unsplash.com/photo-1546538994-4f15d0aa966f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image: 'https://jooinn.com/images/portrait-1.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQCRyi4-dicSyWEFp0un3Taue0spzl0b6fNQA&usqp=CAU',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image: 'https://i.redd.it/7mkdr70e1dl31.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://www.zarias.com/wp-content/uploads/2015/08/Portrait-Photography-Tips-and-Ideas-261.jpg',
          rating: 5,
        },
        {
          title: 'Slide 1',
          image:
            'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQCRyi4-dicSyWEFp0un3Taue0spzl0b6fNQA&usqp=CAU',
          rating: 4.4,
        },
        {
          title: 'Slide 2',
          image: 'https://i.redd.it/7mkdr70e1dl31.jpg',
          rating: 3.5,
        },
        {
          title: 'Slide 3',
          image:
            'https://www.zarias.com/wp-content/uploads/2015/08/Portrait-Photography-Tips-and-Ideas-261.jpg',
          rating: 5,
        },
      ],
    }
  },
}
</script>
<style>
.IMG-F {
  display: block;
  position: relative;
  border-radius: 20px;
  overflow: hidden;
  width: auto;
  height: 15rem;
}
.see-more button {
  border-color:#f6924b;
}
</style>
