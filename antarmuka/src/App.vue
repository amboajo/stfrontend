<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" v-if="isShow">
    
    <h2>hallo</h2>
    Nama Saat ini: {{nama}}
    <br/>
    <input v-model="username" placeholder="masukkan username" id="username"/>
     <br/>
    <input v-model="password" placeholder="masukkan password" id="password"/>
<br/>
<br/>
<br/>
    <button @click="showHide">
      {{ isShow ? 'Hide' : 'Show' }}
      
    </button> -->
    <v-app>
  <v-navigation-drawer app>
    <!-- -->fasfasdasd
  </v-navigation-drawer>

  <v-app-bar app>
    <!-- -->asdasdasd
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>

      <!-- If using vue-router -->
      <router-view></router-view>
    </v-container>
  </v-main>

  <v-footer app>
    <!-- -->asdasdasd
  </v-footer>
</v-app>
  </div>
</template>

<script>

export default {
  beforeCreate() {
    console.log('ini dipanggil before create');
  },

  created() {
    this.nama = 'aldi';
    console.log('ini dipanggil setelah aplikasi dibuat');
  },

  beforeMount() {
    this.nama = 'aldi sebelum mount';
    console.log('before mount dipanggil');
  },

  mounted() {
    console.log('mounted dipanggil');
  },

  data() {
    return{
      nama: 'kosong',
      isShow: true,
      username: '',
      password: ''
    }
  },

  methods: {
    showHide() {
      this.isShow = !this.isShow;
      console.log('ini dipanggil');
    },
    
    
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
