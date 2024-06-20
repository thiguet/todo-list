<script>
import Search from './Search.vue'
import Item from './Item.vue'

export default {
  data() {
    return {
      s: '',
      items: []
    }
  },
  computed: {
    filteredItems() {
        return this.items.filter(item => item.name.includes(this.s));
    } 
  },
  methods: {
    onChangeValue(newValue) {
      this.s = newValue
    }
  },
  async mounted() {
    const response = await fetch('http://localhost:4005/list')
    const items = await response.json()
    
    this.items = items;
  },
  components: {
    Search,
    Item
  }
}
</script>

<template>
  <Search :value="s" :onChangeValue="onChangeValue" />
  <ul>
    <Item v-for="(item, index) in filteredItems" :key="index" v-bind="item" />
  </ul>
</template>
