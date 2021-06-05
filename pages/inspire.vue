<template>
  <section class="section" v-if="info">
    <h1 class="title is-3 has-text-grey">
      {{ info.title }}
    </h1>
    <nuxt-content :document="info" />
  </section>
</template>

<script lang="ts">
import { defineComponent, useContext, useAsync } from '@nuxtjs/composition-api'

export default defineComponent({
  setup () {
    const { $content } = useContext()
    const info = useAsync(() => {
      return $content('hello').fetch()
    })

    return {
      info
    }
  }
})
</script>
