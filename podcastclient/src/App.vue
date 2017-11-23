<template>
  <div id="app">
      <top-header></top-header>
      <div class="container">
          <home></home>
      </div>
  </div>
</template>

<script>
    import TopHeader from './components/TopHeader'
    import Home from './components/Home'

    export default {
      name: 'app',
      components: {
          TopHeader,
          Home
      }
    }
</script>

<style lang="scss">
    @import "~styles/variables";

    * {
        -webkit-box-sizing: border-box;
        -moz-box-sizing: border-box;
        box-sizing: border-box;
    }
    
    body {  
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        color: #2c3e50;
        background-color: #edeff0;
        margin-top: calc(#{$header-height} + (#{$header-padding * 2}));
    }

    p {
        line-height: 1.5;
    }

    .container {
        max-width: 780px;
        margin: 0 auto;
        flex: 1;
    }

    a {
        color: rgba(#387bc9, .9);
        -webkit-transition: color 100ms ease-in;
        -moz-transition: color 100ms ease-in;
        -ms-transition: color 100ms ease-in;
        -o-transition: color 100ms ease-in;
        transition: color 100ms ease-in;


        &:hover {
           color: #387bc9; 
        }
    }

</style>
