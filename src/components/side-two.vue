<template>
  <div class='row' id='side-two'>
    <div class='col-md-4 padding-0' v-for="post in posts">
      <div id='overlay' v-on:click="clicked" ></div>
       <img class="img-fluid img-responsive "  v-bind:src="post.thumbnail" id='some-guy'/>
    </div>

  </div>
</template>

<script>

import axios from 'axios'

export default {
  name: 'side-two',
  data: function () {
    return {
      posts: []
    }
  },
  mounted: function () {
    axios.get('http://hgognavtnecinv44.herokuapp.com/api/posts').then(response => {
      this.posts = response.data.posts.splice(0, 9) })
    },
  methods: {
    clicked: function() {
      this.$parent.$emit('clicked_me')
    }
  }
 }
</script>

<style>

</style>
