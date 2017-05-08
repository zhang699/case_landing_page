<template>
  <div id="app">
    <NavBar />
    <div class="landing-cover">
      <div class="landing-cover-overlay">
        <h1>協助企業開發全端應用程式</h1>
        <button class="border-button">趕快聯絡</button>
      </div>
    </div>
  
    <ServiceContent />

    <Contact />
  </div>
</template>

<script>
import NavBar from './components/NavBar';
import ServiceContent from './components/ServiceContent';
import Contact from './components/Contact';
export default {
  name: 'app',
  components: {
    NavBar,
    ServiceContent,
    Contact,
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
body {
  margin : 0 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.landing-cover {
  background-image: url('./assets/37-usersthink-stock-image.jpg');
  width: 100%;
  height: calc(100vh - 60px);
  background-size: cover;
  position: relative;
  background-position: center center;
  .landing-cover-overlay{
     position: absolute;
     display: flex;
     flex-direction: column;
     justify-content: center;
     color: white;
     width: 100%;
     height: 100%;
     font-weight: 900;
     background-color: rgba(0,0,0,.3);
     .border-button {
       border-style: none;
       border: 2px solid #42b983;
       background-color: #42b983;
       border-radius: 40px;
       outline: none;
       color: white;
       width: 200px;
       height: 45px;
       font-size: 20px;
       align-self: center;
       &:active {
         background-color: white;
         color: black;
         border-color:transparent;
       }
     }
     > h1 {
       padding: 10px;
     }
  }
}
h1, h2 {
}

ul {
  list-style-type: none;
  padding: 0;
}

hr {
  border: none;
  border-bottom: 4px solid white;
  width: 100px;
  margin: 0 0;
  margin-left: 20px;
  border-radius: 10px;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.header {
  margin-left: 20px;
}

a {
  color: #42b983;
}
</style>
