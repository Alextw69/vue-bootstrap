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
        </b-container>
        <b-container>
            <b-button @click="change_aspect('2:1')" class="m-3">2:1</b-button>
            <b-button @click="change_aspect('4:3')" class="m-3">4:3</b-button>
            <b-button @click="change_aspect('16:9')" class="m-3">16:9</b-button>
            <b-button @click="change_aspect('1.85:1')" class="m-3">1.85:1</b-button>

            <hr />

            <b-aspect :aspect="aspect" style="border: 1px solid black;">
              My aspect: {{aspect}}
            </b-aspect>

            <hr />

            <b-row>
                  <b-col>
                    <b-aspect :aspect="aspect" style="border: 1px solid black;">
                      My aspect: {{aspect}}
                    </b-aspect>
                  </b-col>
                  <b-col>
                    <b-aspect :aspect="aspect" style="border: 1px solid black;">
                      My aspect: {{aspect}}
                    </b-aspect>
                  </b-col>
            </b-row>
        </b-container>
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
        aspect: '2:1',
     } 
  },
  methods:{
     toggle_success_alert(){
        this.success_show = !this.success_show;
     },
      change_aspect (aspect_value) {
      this.aspect = aspect_value;
    }
  }
  // components: {
  //    HelloWorld
  // }
}
</script>
