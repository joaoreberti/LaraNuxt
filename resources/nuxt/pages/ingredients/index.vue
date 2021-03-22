<template>
  <div>
    <v-text-field color="white" v-model="search" label="Ingredientes..." dark
      >default slot</v-text-field
    >

    <div class="d-flex flex-wrap">
      <v-card
        width="calc(100% / 5)"
        v-for="(ingredient, i) in ingredients"
        :key="i"
        @click="$router.push(`/ingredients/${ingredient.id}`)"
      >
        <v-img height="250" :src="ingredient.imgUrl"></v-img>
        <v-card-title>{{ ingredient.name }}</v-card-title>
        <v-card-text>{{ ingredient.description }}</v-card-text>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      search: '',
      ingredients: [
        {
          id: 1,
          name: 'banana',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 2,
          name: 'laranja',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 3,
          name: 'maça',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 4,
          name: 'pêra',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 5,
          name: 'vitela',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 6,
          name: 'frango',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 7,
          name: 'porco',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 8,
          name: 'pescado',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 9,
          name: 'bacalhau',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 10,
          name: 'salmão',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 11,
          name: 'borrego',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        },
        {
          id: 12,
          name: 'tomamte',
          imgUrl: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
          description: 'lorem ipsum '
        }
      ]
    }
  },
  methods: {
    filterSearch() {}
  }
}
</script>

<style lang="scss" scoped></style>
