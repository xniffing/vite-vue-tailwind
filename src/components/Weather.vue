<template>
  <div>{{ collectionName }}: {{ readersNumber }} {{ book.title }}</div>
  <input type="text" v-model="book.title"/>

</template>

<script>
  import { ref, reactive } from 'vue'

  export default {
    props: {
      collectionName: String
    },
    setup(props) {
      const readersNumber = ref(props.collectionName.length)
      const book = reactive({ title: 'Vue 3 Guide' })

      // expose to template
      return {
        readersNumber,
        book
      }
    }
  }
</script>
