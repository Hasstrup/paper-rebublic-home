<template>
  <div id="app">

    <div class='row' id='home-row'>
      <div class='col-md-6'>
        <div id='side-one'>
          <side-one :headerOne='header1' :headerTwo='header2'/>
        </div>

      </div>

      <div class='col-md-6'>
        <div id='side-two'>
          <side-two/>
        </div>


      </div>

    </div>
  </div>
</template>

<script>
import SideOne from './components/side-one'
import SideTwo from './components/side-two'
export default {
  name: 'app',
  components: {
    'side-one': SideOne,
    'side-two': SideTwo
  },
  data: function () {
    return {
      header1: 'Of Course',
      header2: "It's not your phone, it's you"
    }},

  events: {
    'clicked_me': function() {
    alert('clicked me')
    }
  },
  

  created: function() {
    this.$on('clicked_me', function(){
      this.header1 = 'Oh you like that?',
      this.header2 = "We thought so too"
      this.change_back();
})
},

methods: {
      change_back: function(){
        setTimeout(() =>  {
        this.header1 = 'Of Course',
        this.header2 = "It's not your phone, it's you"
      }, 2000)
    }}

}
</script>

<style>



</style>
