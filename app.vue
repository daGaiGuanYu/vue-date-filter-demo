<template lang="pug">
  div
    div {{haha}}
    div {{haha | formatDate}}
    div {{haha | haha}}
    div {{heihei | go}}
</template>

<script>
import Vue from 'vue'

Vue.filter( 'formatDate', value => {
  return new Date(value)
})

Vue.filter( 'haha', value => {
  return 999
})

export default {
  data(){
    return {
      haha: '2018-10-29',
      heihei: 'nihao'
    }
  }
}
</script>