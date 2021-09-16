<template>
    <!-- <div class="home"> -->
    <b-container>

        <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
        <b-button variant="success" class="m-3">使用-bootstrap-vue</b-button>
        <!-- <b-container class="bv-example-row">
        <b-row>
            <b-col>1 of 3</b-col>
            <b-col>2 of 3</b-col>
            <b-col>3 of 3</b-col>
            <div>
                <b-alert show>Default Alert</b-alert>
                <b-alert variant="success" show>Success Alert</b-alert>
            </div>
        </b-row>
        </b-container>
        <b-container fluid>
              <b-col >1 of 3</b-col>
              <b-col>2 of 3</b-col>
              <b-col>3 of 3</b-col>
        </b-container> -->
        <b-container>
            <div>
                <b-alert show>Default Alert</b-alert>
                <b-alert variant="success" show>Success Alert</b-alert>
                <!-- <b-alert variant="danger" show>danger Alert</b-alert>
                <b-alert variant="warning" show>warning Alert</b-alert> -->
            </div>
            <div>
                <b-alert variant="success"  :show="success_show">Toggle now</b-alert>
                <b-button @click="toggle_success_alert">Toggle success alert</b-button>
                <hr>
                <b-alert show variant="danger" dismissible>Danger alert with dismissible</b-alert>
            </div>
            <hr>
            <div class="mb-4">
              <b-avatar></b-avatar>
              <b-avatar variant="primary" text="BV"></b-avatar>
              <b-avatar variant="info" src="https://placekitten.com/300/300" class="m-2" size=""></b-avatar>
              <b-avatar variant="info" src="https://placekitten.com/310/310" class="m-2" size="24px"></b-avatar>
              <b-avatar variant="info" src="https://placekitten.com/320/320" class="m-2" :size="42"></b-avatar>
              <b-avatar variant="info" src="https://placekitten.com/330/330" class="m-2" size="6rem"></b-avatar>
              <b-avatar variant="success" icon="people-fill"></b-avatar>
            </div>
            <div class="mb-2">
              <b-avatar icon="people-fill"></b-avatar>
              <b-avatar icon="star-fill"></b-avatar>
              <b-avatar icon="music-note"></b-avatar>
              <b-avatar icon="star-fill" size="4em"></b-avatar>
            </div>
            <div>
              <b-avatar variant="secondary"></b-avatar>
              <b-avatar variant="primary"></b-avatar>
              <b-avatar variant="dark"></b-avatar>
              <b-avatar variant="light"></b-avatar>
              <b-avatar variant="success"></b-avatar>
              <b-avatar variant="danger"></b-avatar>
              <b-avatar variant="warning"></b-avatar>
              <b-avatar variant="info"></b-avatar>
            </div>
            <b-button pill variant="outline-primary" class="m-2">Outline - Primary</b-button>
            <b-button squared variant="outline-success" class="m-2">Outline - Success</b-button>
            <b-button variant="outline-danger" class="m-2">Outline - Danger</b-button>
            <b-button variant="outline-warning" class="m-2">Outline - Warning</b-button>
        </b-container>
        <!-- <b-container>
            <b-button @click="change_aspect('2:1')" class="m-3">2:1</b-button>
            <b-button @click="change_aspect('4:3')" class="m-3">4:3</b-button>
            <b-button @click="change_aspect('16:9')" class="m-3">16:9</b-button>
            <b-button @click="change_aspect('1.85:1')" class="m-3">1.85:1</b-button>

            <hr />

            <b-aspect :aspect="aspectkk" style="border: 1px solid black;">
              My aspect: {{aspectkk}}
            </b-aspect>

            <hr />

            <b-row>
                  <b-col>
                    <b-aspect :aspect="aspectkk" style="border: 1px solid black;">
                      My aspect: {{aspectkk}}
                    </b-aspect>
                  </b-col>
                  <b-col>
                    <b-aspect :aspect="aspectkk" style="border: 1px solid black;">
                      My aspect: {{aspectkk}}
                    </b-aspect>
                  </b-col>
            </b-row>
        </b-container> -->
      </b-container>

</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  data(){
     return {
        success_show : false,
        aspectkk: '2:1',
     } 
  },
  methods:{
     toggle_success_alert(){
        this.success_show = !this.success_show;
     },
      change_aspect (aspect_value) {
      this.aspectkk = aspect_value;
    }
  }
  // components: {
  //    HelloWorld
  // }
}
</script>
