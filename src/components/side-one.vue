<template>
  <div>
    <div id='container-ting'>
      <h1 id='span-me'> {{ headerOne }} </h1>
      <h2> {{ headerTwo }}</h2>
    </div>
     <hr id='hr-ting'/>

     <div id='align-text'>
       <h6 id='id-me'> We're tacitly collaborating with designers, photographers
            and <br/> content creators all over the world,<br/> to bring
         the most artsy content to your lockscreen. <br/>Enjoy all this and more and getting the application
         <br/> from the <a id='button-ting' href='/'> Play Store </a> now.
       </h6>
     </div>

  </div>
</template>

<script>
  export default {
    name: 'side-one',
    data: function () {
      return {
        title: " it's not your lockscreen. It's you"
      }
    },
    props: ['headerOne', 'headerTwo' ]

  }
</script>
