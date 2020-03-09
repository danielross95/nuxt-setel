<template>
  <div @input="updateHTML" contenteditable="true" class="textEditor"></div>
</template>
<script>
export default {
  name: 'TextEditor',
  props: {
    value: undefined
  },
  data() {
    return {
      test: 'H<b>ELLO</b> <i>Wor</i>ld!'
    }
  },
  mounted() {
    this.$el.innerHTML = this.value
  },
  methods: {
    updateHTML(e) {
      this.$emit('input', e.target.innerHTML)
    }
  }
}
</script>
<style scoped>
.textEditor {
  border: 1px solid lightblue;
  min-height: 42px;
  padding: 1rem 1.35rem;
}
</style>
