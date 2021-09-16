<template>
 
  <b-container class="bv-example-row">
      <b-navbar toggleable type="dark"  class="mb-3 nav-background">
            <b-navbar-brand href="#" >NavBar</b-navbar-brand>

            <b-navbar-toggle target="navbar-toggle-collapse">
              <template #default="{ expanded }">
                <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
                <b-icon v-else icon="chevron-bar-down"></b-icon>
              </template>
            </b-navbar-toggle>

            <b-collapse id="navbar-toggle-collapse" is-nav>
                <b-navbar-nav class="ml-auto nav-background">
                    <b-nav-item href="#" >Link 1</b-nav-item>
                    <b-nav-item href="#" >Link 2</b-nav-item>
                    <b-nav-item href="#" >Link 3</b-nav-item>
                    <b-nav-item href="#" >Link 4</b-nav-item>
                    <b-nav-item href="#" disabled>Disabled</b-nav-item>
                </b-navbar-nav>
            </b-collapse>
      </b-navbar>

      <b-breadcrumb class="breadcrumb">
        <b-breadcrumb-item href="#Home">Home</b-breadcrumb-item>
        <b-breadcrumb-item href="#Blog">Blog</b-breadcrumb-item>
        <b-breadcrumb-item active>Hello World!</b-breadcrumb-item>
      </b-breadcrumb>

       <b-row>
            <b-col  cols="3">
                <b-button variant="success" class="">使用-bootstrap-vue</b-button><br>
                <b-button pill variant="warning" class="m-3">使用-bootstrap-vue</b-button>
                <b-button variant="danger">使用-bootstrap-vue</b-button>
            </b-col>
            <b-col  cols="3">
                  cols="?" cols="?" amet consectetur, adipisicing elit. Repudiandae, illum earum. Quam asperiores harum, repellendus dolorum earum molestias. Necessitatibus perspiciatis alias consequuntur amet nihil officiis quisquam, dignissimos excepturi. Vel, commodi.
            </b-col>
            <b-col  cols="3" class="nav-background">
                  Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae, illum earum. Quam asperiores harum, repellendus dolorum earum molestias. Necessitatibus perspiciatis alias consequuntur amet nihil officiis quisquam, dignissimos excepturi. Vel, commodi.
            </b-col>
            <b-col  cols="3">
                  Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae, illum earum. Quam asperiores harum, repellendus dolorum earum molestias. Necessitatibus perspiciatis alias consequuntur amet nihil officiis quisquam, dignissimos excepturi. Vel, commodi.
            </b-col>
       </b-row>
       <hr>
       <b-row>
            <b-col md="4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Et tempore, illum minima adipisci voluptatum dolorum. Beatae fugit placeat qui quidem totam tempore enim voluptatibus magnam. Perferendis beatae rem eligendi vitae?</b-col>
            <b-col md="4" offset-md="4">offset-md="4" offset-md="4" consectetur adipisicing elit. Fugit corporis illum animi, ducimus obcaecati corrupti quisquam iure, saepe illo, qui sequi sapiente voluptatem amet repellendus quis. Voluptas illo officia rem.</b-col>
       </b-row>
       <hr>
       <b-row>
            <b-col md="4">  
                 <b-card
                    title="Card Title"
                    img-src="https://picsum.photos/600/300/?image=25"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="mb-2">
                      <b-card-text>
                          Some quick example text to build on the card title and make up the bulk of the card's content.
                      </b-card-text>
                      <b-button href="#" variant="primary">Go somewhere</b-button>
                 </b-card>
            </b-col>
            <b-col md="4" > 
                 <b-card
                    title="Card Title"
                    img-src="https://picsum.photos/600/300/?image=25"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="mb-2"
                  >
                    <b-card-text>
                         Some quick example text to build on the card title and make up the bulk of the card's content.
                    </b-card-text>
                    <b-button href="#" variant="primary">Go somewhere</b-button>
                 </b-card>
            </b-col>
            <b-col md="4"> 
                 <b-card
                    title="Card Title"
                    img-src="https://picsum.photos/600/300/?image=25"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="mb-2">
                    <b-card-text>
                         Some quick example text to build on the card title and make up the bulk of the card's content.
                    </b-card-text>
                    <b-button href="#" variant="primary">Go somewhere</b-button>
                 </b-card>
            </b-col>
       </b-row>
       <hr>
       <b-row>
          <b-col>
              <b-card title="Card title" sub-title="Card subtitle"  class="mb-2">
                  <b-card-text>
                    Some quick example text to build on the <em>card title</em> and make up the bulk of the card's
                    content.
                  </b-card-text>

                  <b-card-text>A second paragraph of text in the card.</b-card-text>

                  <a href="#" class="card-link">Card link</a>
                  <b-link href="#" class="card-link">Another link</b-link>
              </b-card>
          </b-col>
          <b-col>
              <b-card title="Card title" sub-title="Card subtitle">
                  <b-card-text>
                    Some quick example text to build on the <em>card title</em> and make up the bulk of the card's
                    content.
                  </b-card-text>

                  <b-card-text>A second paragraph of text in the card.</b-card-text>

                  <a href="#" class="card-link">Card link</a>
                  <b-link href="#" class="card-link">Another link</b-link>
              </b-card>
          </b-col>
          <b-col>
              <b-card title="Card title" sub-title="Card subtitle">
                  <b-card-text>
                      Some quick example text to build on the <em>card title</em> and make up the bulk of the card's
                      content.
                  </b-card-text>

                  <b-card-text>A second paragraph of text in the card.</b-card-text>

                  <a href="#" class="card-link">Card link</a>
                  <b-link href="#" class="card-link">Another link</b-link>
              </b-card>
          </b-col>
       </b-row>
       <hr>
       <b-card    overlay
                  img-src="https://picsum.photos/900/350/?image=1"
                  img-alt="Card Image"
                  text-variant="white"
                  title="Image Overlay"
                  sub-title="Subtitle"
                  class="mb-2">
          <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
          </b-card-text>
      </b-card>
      <b-carousel
            v-model="slide"
            :interval="2000"
            controls
            indicators
            fade
            img-width="1024"
            img-height="480"
            @sliding-start="onSlideStart"
            @sliding-end="onSlideEnd"
            class="mb-5"
          >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="First slide"
        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
        img-src="https://picsum.photos/1024/480/?image=14"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=13">
        <h1>Hello world!</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=11"></b-carousel-slide>
    </b-carousel>
    <hr>
            <b-button v-b-toggle.collapse-1 variant="primary">Toggle Collapse</b-button>
            <b-collapse id="collapse-1" class="mb-2">
              <b-card>
                <p class="card-text">Collapse-1 contents Here</p>
              </b-card>
            </b-collapse>
    <hr>
            <b-button v-b-toggle.collapse-2 variant="success">Toggle Collapse</b-button>
            <b-collapse id="collapse-2" class="mb-2">
              <b-card>
                <p class="card-text">Collapse-2 contents Here</p>
                <b-button v-b-toggle.collapse-2-inner size="sm">Toggle Inner Collapse</b-button>
                <b-collapse id="collapse-2-inner" class="mb-2">
                    <b-card>Hello! collapse-3 </b-card>
                </b-collapse>
              </b-card>
            </b-collapse>
    <hr>
    <b-button v-b-toggle.collapse-group variant="primary" class="mb-2">Toggle Collapse Group</b-button>

        <b-collapse id="collapse-group">
            <b-card no-body class="mb-1" >
                <b-card-header header-tag="header" class="p-1">
                    <b-button block v-b-toggle.tab-1 variant="warning">Tab 1</b-button>
                </b-card-header>
                <b-collapse id="tab-1" accordion="my-group" visible>
                    <b-card-body>Tab text 1</b-card-body>
                </b-collapse>
            </b-card>

            <b-card no-body class="mb-1" >
                <b-card-header header-tag="header" class="p-1">
                    <b-button block v-b-toggle.tab-2 variant="info">Tab 2</b-button>
                </b-card-header>
                <b-collapse id="tab-2" accordion="my-group">
                    <b-card-body>Tab text 2</b-card-body>
                </b-collapse>
            </b-card>

            <b-card no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1">
                    <b-button block v-b-toggle.tab-3 variant="info">Tab 3</b-button>
                </b-card-header>
                <b-collapse id="tab-3" accordion="my-group">
                    <b-card-body>Tab text 3</b-card-body>
                </b-collapse>
            </b-card>
        </b-collapse>
        <hr/>
        Aspect: <code>21by9 (21:9)</code>, <code>16by9 (16:9)</code>, <code>4by3 (4:3)</code>, <code>1by1 (1:1)</code>
        <hr />
        <code>16:9</code>
        <b-embed
            type="iframe"
            aspect="16by9"
            src="https://www.youtube.com/embed/IOclm64OyWI"
            allowfullscreen
        ></b-embed>

        <hr />

        <code>4:3</code>
        <b-embed
            type="video" aspect="4by3"
            controls
            poster="https://placekitten.com/1024/768"
        >
            <source src="dev-stories.webm" type="video/webm">
            <source src="dev-stories.mp4" type="video/mp4">
        </b-embed>

  </b-container>
</template>

<script>
    export default {
      data() {
          return {
            slide: 0,
            sliding: null
          }
        },
        methods: {
            onSlideStart(slide) {
              this.sliding = true
            },
            onSlideEnd(slide) {
              this.sliding = false
            }
        }
      }
</script>
<style scoped>
    h1{
      color:chartreuse;
    }
    .nav-background{
      background: rgb(221, 236, 12);
    }
    .breadcrumb{
      background: rgb(225, 187, 226);
      display: inline-flex;
    }
</style>