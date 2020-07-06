<template>
  <div class="body">
    <button @click="getMockUser">ccc</button>
  </div>
</template>

<script>
export default {
  name: '',
  props: [''],
  data() {
    return {}
  },

  components: {},

  computed: {},

  methods: {
    getMockUser() {
      let res = this.$axios.get('user.json').then((res) => {
        console.log('GET MOCK USER====', res)
      })
    }
  },

  watch: {},

  beforeMount() {},

  mounted() {},

  created() {}
}
</script>
<style lang="scss" scoped></style>
