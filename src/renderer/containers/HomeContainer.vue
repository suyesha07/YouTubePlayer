<template>
  <home :actions="actions" :state="state"></home>
</template>

<script lang="ts">
import Vue from "vue";
import Component from 'vue-class-component'
import Home from '../components/Home.vue'

@Component({
  components: { "home": Home },
  props: {
    actions: { type: Object, required: true },
    state: { type: Object, required: true },
    getters: { type: Object, required: true }
  }
})
export default class HomeContainer extends Vue {
}
</script>
