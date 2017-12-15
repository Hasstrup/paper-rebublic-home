<template>
  <div>
    <div id='header'>
       <div id='header-logo'>
         <h6 class='header-tingg'> Paper-Stack</h6>
       </div>
       <div id='header-twitter'>
         <a href='https://twitter.com/getpaperstack'>
         <svg id="i-twitter" viewBox="0 0 64 64" >
           <path stroke-width="0" fill="#48C9B0" d="M60 16 L54 17 L58 12 L51 14 C42 4 28 15 32 24 C16 24 8 12 8 12 C8 12 2 21 12 28 L6 26 C6 32 10 36 17 38 L10 38 C14 46 21 46 21 46 C21 46 15 51 4 51 C37 67 57 37 54 21 Z" />
         </svg>
         </a>
     </div>
    </div>
    <div class='wrapper'>
    <div id='container-ting'>
      <h1 id='span-me'> {{ headerOne }} </h1>
      <h2 id='span-me2'> {{ headerTwo }}</h2>
    </div>
     <hr id='hr-ting'/>

     <div id='align-text'>
       <h6 id='id-me'> We're tacitly collaborating with designers, photographers
            and <br/> content creators all over the world,<br/> to bring
         the most artsy content to your lockscreen. <br/>Enjoy all this and more by getting the application
         <br/> from the <a id='button-ting' href='/'> Play Store </a>  and <a id='button-ting' href='/'> App Store </a>  now.
       </h6>
     </div>
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
