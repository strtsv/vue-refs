<template>
  <div>
    <h1>Hello Vue!</h1>
    <input type='text' ref='name'/>
    <button @click='focus'>Focus input</button>
  </div>

</template>

<script>
export default {
  methods: {
    focus () {
      console.log('here will be focus', this.$refs.name)
      this.$refs.name.focus()
    }
  }
}
</script>
