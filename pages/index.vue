<template>
  <section class="section">
    <div class="title">
      <strong>JASA</strong>
    </div>
    <b-carousel-list v-model="test" :data="items" :items-to-show="4">
      <template slot="item" slot-scope="list">
        <div class="card CD-J">
          <div class="card-image">
            <figure class="image is-4by5">
              <a @click="list.index;"><img :src="list.image" /></a>
            </figure>
            <!-- <b-tag type="is-danger" rounded style="position: absolute; top: 0;"><b>50%</b></b-tag> -->
          </div>
          <div class="card-content">
            <div class="content">
              <div class="content columns mb-0 is-mobile">
                <div class="column">
                  <div class="PHOTO-PROFILE container">
                    <img
                      src="https://raw.githubusercontent.com/AmzyZy24/Item/master/no-icon.png"
                      alt=""
                      width="100%"
                    />
                    <div class="DOT-STATUS container"></div>
                  </div>
                </div>
                <div class="INFO column is-full pl-1">
                  <div class="is-size-5 has-text-weight-semibold px-1">
                    <p class="title is-6">{{ list.title }}</p>
                  </div>
                  <div
                    class="is-one-fifth is-size-7 has-text-weight-normal px-1"
                  >
                    Mitra level <span>2</span>
                  </div>
                </div>
              </div>
              <div class="content columns mb-0 is-mobile">
                <div class="column">
                  <p class="subtitle is-7">Make your dreams come true and standing apart on this imagination</p>
                </div>
              </div>
              <!-- <p class="subtitle is-7">Make your dreams come true and standing apart on this imagination</p> -->
              <div class="field name-mr is-grouped mb-2 is-mobile">
                <p class="control" v-if="list.rating">
                  <b-rate
                    :value="list.rating"
                    show-score
                    disabled
                    :max="maxs"
                    :v-show="score"
                  >
                  </b-rate>
                </p>
                <p>(23 reviews)</p>
              </div>
              <div class="field is-grouped is-mobile">
                <p class="control" style="margin-right: auto;">
                  <button class="button is-small is-danger is-outlined">
                    <b-icon size="is-small" icon="heart" />
                  </button>
                </p>
                <p class="cotent" style="margin-left: auto;">
                  Price Start = $23
                </p>
                
              </div>
            </div>
          </div>
        </div>
      </template>
    </b-carousel-list>
    <div class="title">
      <strong>JASA</strong>
    </div>
    <b-carousel-list v-model="test" :data="items" :items-to-show="4">
      <template slot="item" slot-scope="list">
        <div class="card CD-J">
          <div class="card-image">
            <figure class="image is-4by5">
              <a @click="list.index;"><img :src="list.image" /></a>
            </figure>
            <!-- <b-tag type="is-danger" rounded style="position: absolute; top: 0;"><b>50%</b></b-tag> -->
          </div>
          <div class="card-content">
            <div class="content">
              <p class="title is-6">{{ list.title }}</p>
              <p class="subtitle is-7">@johnsmith</p>
              <div class="field is-grouped">
                <p class="control" v-if="list.rating">
                  <b-rate
                    :value="list.rating"
                    show-score
                    disabled
                    :max="maxs"
                    :v-show="score"
                  >
                  </b-rate>
                </p>
                <p class="control" style="margin-left: auto;">
                  <button class="button is-small is-danger is-outlined">
                    <b-icon size="is-small" icon="heart" />
                  </button>
                </p>
              </div>
            </div>
          </div>
        </div>
      </template>
    </b-carousel-list>
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
      score: 'true',
      maxs: 1,
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
.see-more button {
  border-color: #f6924b;
}
.carousel-list .carousel-slides .carousel-slide {
  border: 2px solid transparent;
  -ms-flex-negative: 0;
  flex-shrink: 0;
  padding: 1%;
}
.card-content {
  background-color: transparent;
  padding: 0.5rem;
}
.DOT-STATUS {
  width: 8px;
  height: 8px;
  background-color: greenyellow;
  border-radius: 290486px;
  position: absolute;
  bottom: 1px;
  right: 1px;
}
.PHOTO-PROFILE {
  width: 2.7rem;
  height: 2.7rem;
  border-color: #f79351;
  border-width: thin;
  border-style: solid;
  border-radius: 290486px;
}
</style>
