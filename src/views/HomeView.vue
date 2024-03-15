<template>
  <v-app
    id="home"
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
    <navbar-component />
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="1b.png" contain max-height="500"></v-img>
        </v-col>
        <v-col cols="6">
          <h3 class="red--text text-darken-4 top">Hello I am Priyanshu</h3>
          <h1 class="white--text">Software Developer</h1>
          <p class="grey--text">
            I am a computer science graduate working as a Front-end
            Developer.<br />
            My passion for technology and eagerness to learn new things has
            driven me <br /> to stay upto date with the latest industry trends and
            tools. <br />
            I have experience working with popular web frameworks such as Vue, <br />
            Nuxt, React, Express, and Node.js, and I am always looking for
            opportunities <br /> to expand my skillset. 
            As a quick learner with a strong work ethic, <br />
             I am confident that I can make a valuable contribution to your team. <br />
              I am excited about the opportunity to apply my skills and knowledge to real world
            projects, <br /> and I am eager to take on new challenges as a software
            developer.
          </p>
          <!-- About me section-->
          <!-- <v-btn tile color="#A7121D" dark>About me</v-btn> -->
          <v-dialog
            v-model="aboutMeDialog"
            persistent
            max-width="600"
            max-height="400"
          >
            <template v-slot:activator="{ on, attrs }">
              <v-btn tile color="#A7121D" dark v-bind="attrs" v-on="on">
                About Me
              </v-btn>
            </template>
            <v-card color="#1e1e1e" dark>
              <h3 class="white--text pl-3 pt-6">
                Hi, I’m Priyanshu. Nice to meet you.
              </h3>
              <p class="grey--text pl-3 mt-3">
                I am a Software Developer at Global Ids. I have one year of
                experience in web development, with expertise in Vue.js,
                Vuetify, Node.js, Express, Mongo, Java, Javascript and Tailwind
                Css. As a Frontend Developer at Global Ids, I was responsible
                for developing and maintaining web applications for various
                clients, using Vue.js as the main framework. I have also used
                Vuetify and Tailwind Css to create responsive and user-friendly
                interfaces, Node.js and Express to handle backend logic, and
                MongoDB to store and manage data.
              </p>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn
                  color="blue darken-1"
                  text
                  @click="aboutMeDialog = false"
                >
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-dialog>
        </v-col>
        <v-col cols="12" class="padd">
          <div class="first" id="about">
            <v-row>
              <v-col cols="12">
                <div
                  class="child bgColor1"
                  onmouseover="this.classList.add('bgColor2')"
                  onmouseout="this.classList.remove('bgColor2')"
                >
                  <v-icon x-large class="ml-3">mdi-pencil-ruler</v-icon>
                  <h3 class="white--text ml-3 mt-6">UI Design</h3>
                  <p class="grey--text ml-3 mt-6">
                    I like creating visually appealing and <br />
                    user-friendly interfaces for digital products
                  </p>
                  <!-- <v-btn dark text>
                    know more
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn> -->
                  <v-dialog
                    v-model="designDialog"
                    persistent
                    max-width="600"
                    max-height="400"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn dark text v-bind="attrs" v-on="on">
                        know more
                        <v-icon right>mdi-arrow-right</v-icon>
                      </v-btn>
                    </template>
                    <v-card color="#1e1e1e" dark>
                      <h3 class="white--text pl-3 pt-6">
                        User Interface Designing
                      </h3>
                      <p class="grey--text pl-3 mt-3">
                        I like creating visually appealing and user-friendly
                        interfaces for digital products
                      </p>
                      <h3 class="white--text pl-3 mt-3">Design Elements :</h3>
                      <p class="grey--text pl-3 mt-3">
                        UX, UI, Web, Apps, Logos
                      </p>
                      <h3 class="white--text pl-3 mt-3">Design Tools :</h3>
                      <p class="grey--text pl-3 mt-3">
                        Adobe Photoshop, Figma, Pen & Paper, Sketch, Webflow
                      </p>
                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="blue darken-1"
                          text
                          @click="designDialog = false"
                        >
                          Close
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
                <div
                  class="child bgColor1"
                  onmouseover="this.classList.add('bgColor2')"
                  onmouseout="this.classList.remove('bgColor2')"
                >
                  <v-icon x-large class="ml-3" dark>mdi-web</v-icon>
                  <h3 class="white--text ml-3 mt-4">Frontend Developer</h3>
                  <p class="grey--text ml-3 mt-6">
                    I like to code things from scratch and enjoy <br />
                    bringing ideas to life in the browser.
                  </p>
                  <!-- <v-btn dark text>
                    know more
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn> -->
                  <v-dialog
                    v-model="frontendDialog"
                    persistent
                    max-width="600"
                    max-height="400"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn dark text v-bind="attrs" v-on="on">
                        know more
                        <v-icon right>mdi-arrow-right</v-icon>
                      </v-btn>
                    </template>
                    <v-card color="#1e1e1e" dark>
                      <h3 class="white--text pl-3 pt-6">
                        Frontend Development
                      </h3>
                      <p class="grey--text pl-3 mt-3">
                        I like to code things from scratch and enjoy bringing
                        ideas to life in the browser.
                      </p>
                      <h3 class="white--text pl-3 mt-3">Languages :</h3>
                      <p class="grey--text pl-3 mt-3">
                        JavaScript/TypeScript, HTML, Css, Sass, Git
                      </p>
                      <h3 class="white--text pl-3 mt-3">
                        Tools and Technologies :
                      </h3>
                      <p class="grey--text pl-3 mt-3">
                        Vue.js, React.js, Vuetify, Nuxt.js, Tailwind Css,
                        Bootstrap, GitHub, VS Code, Netlify
                      </p>
                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="blue darken-1"
                          text
                          @click="frontendDialog = false"
                        >
                          Close
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
                <div
                  class="child bgColor1"
                  onmouseover="this.classList.add('bgColor2')"
                  onmouseout="this.classList.remove('bgColor2')"
                >
                  <v-icon x-large class="ml-3">mdi-code-json</v-icon>
                  <h3 class="white--text ml-3 mt-4">Backend Developer</h3>
                  <p class="grey--text ml-3 mt-6">
                    I like creating and maintaining the server-side <br />
                    logic of a software application.
                  </p>
                  <v-dialog
                    v-model="backendDialog"
                    persistent
                    max-width="600"
                    max-height="400"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn dark text v-bind="attrs" v-on="on">
                        know more
                        <v-icon right>mdi-arrow-right</v-icon>
                      </v-btn>
                    </template>
                    <v-card color="#1e1e1e" dark>
                      <h3 class="white--text pl-3 pt-6">Backend Development</h3>
                      <p class="grey--text pl-3 mt-3">
                        I like creating and maintaining the server-side logic of
                        a software application.
                      </p>
                      <h3 class="white--text pl-3 mt-3">Languages :</h3>
                      <p class="grey--text pl-3 mt-3">
                        Java, Python, Node.js, Sql
                      </p>
                      <h3 class="white--text pl-3 mt-3">
                        Tools and Technologies :
                      </h3>
                      <p class="grey--text pl-3 mt-3">
                        IntelliJ, CLion/PyCharm/IDEA, Atom, Spring, SpringBoot,
                        Node.js, Express.js, MongoDB
                      </p>
                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="blue darken-1"
                          text
                          @click="backendDialog = false"
                        >
                          Close
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </v-col>
              <v-col cols="12" class="mt-10">
                <div class="child1">
                  <h1 class="red--text text-darken-4 mt-4 number">1+</h1>
                  <h3 class="white--text mt-4">Years Experience</h3>
                </div>
                <div class="child2 mRight">
                  <v-row>
                    <v-col cols="12" class="childcol">
                      <div class="child2 mButton padding bgColor1">
                        <p class="red--text text--darken-4">Global Ids</p>
                        <p class="grey--text">Software Developer</p>
                      </div>
                    </v-col>
                    <v-col cols="12" class="childcol">
                      <div class="child2 padding bgColor1">
                        <p class="red--text text--darken-4">
                          Persistent Systems
                        </p>
                        <p class="grey--text">Java Software Developer</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>
                <div class="child2">
                  <v-row>
                    <v-col cols="12" class="childcol">
                      <div class="child2 mButton padding bgColor1">
                        <p class="red--text text--darken-4">10+ months</p>
                        <p class="grey--text">Relevant Experience</p>
                      </div>
                    </v-col>
                    <v-col cols="12" class="childcol">
                      <div class="child2 padding bgColor1">
                        <p class="red--text text--darken-4">6 months</p>
                        <p class="grey--text">Internship Experience</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col md="3" offset-md="3" id="project">
          <h4 class="white--text">FEATURED PROJECTS</h4>
          <p class="grey--text">
            These are some of the projects I have worked on
          </p>
        </v-col>
        <v-col md="3" class="text-end">
          <a href="https://github.com/Kraken-ops">
          <v-btn tile color="#A7121D" dark>
            <v-icon left>mdi-github</v-icon>
            View All
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </a>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-card
            class="pa-2 py-12"
            outlined
            tile
            height="250px"
            color="#1E1E1E"
          >
            <v-img
              src="3a.png"
              contain
              min-height="100"
              min-width="200"
              max-height="200"
              max-width="400"
            ></v-img>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card
            class="pa-2 py-12"
            outlined
            tile
            height="250px"
            color="#1E1E1E"
          >
            <v-img
              src="3b.png"
              contain
              min-height="100"
              min-width="200"
              max-height="200"
              max-width="400"
            ></v-img>
          </v-card>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-btn color="white" dark text class="ml-n4">Project Beti</v-btn
          ><br />
          <a href="https://projectbeti.web.app/">
  <v-btn color="#A7121D" dark text class="ml-n4">
    know more
    <v-icon right>mdi-arrow-right</v-icon>
  </v-btn>
</a>
        </v-col>

        <v-col md="3">
          <v-btn color="white" dark text class="ml-n4">Ingenium</v-btn><br />
          <a href="https://aotingenium.com/archive/">
          <v-btn color="#A7121D" dark text class="ml-n4"
            >know more
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </a>
        </v-col>

        <v-col md="3" offset-md="3">
          <v-card
            class="pa-2 py-12"
            outlined
            tile
            height="250px"
            color="#1E1E1E"
          >
            <v-img
              contain
              src="4a.png"
              min-height="100"
              min-width="200"
              max-height="200"
              max-width="400"
            ></v-img>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card
            class="pa-2 py-12"
            outlined
            tile
            height="250px"
            color="#1E1E1E"
          >
            <v-img
              src="4b.png"
              contain
              min-height="100"
              min-width="200"
              max-height="200"
              max-width="400"
            ></v-img>
          </v-card>
        </v-col>

        <v-col md="3" offset-md="3">
          <v-btn color="white" dark text class="ml-n4">Ecommerce Website</v-btn
          ><br />
          <v-btn color="#A7121D" dark text class="ml-n4"
            >know more
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>

        <v-col md="3">
          <v-btn color="white" dark text class="ml-n4">Sales Dashboard</v-btn
          ><br />
          <v-btn color="#A7121D" dark text class="ml-n4"
            >know more
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>

        <v-col cols="12" class="padd topInverse">
          <div class="second">
            <div class="secondChild1" id="contact">
              <v-row>
                <v-col cols="7">
                  <h1 class="white-text">
                    Thank you for going through my website.
                  </h1>
                  <p class="grey-text">
                    I hope you have found my website clean, minimal, interesting
                    and intuitive. Feel free to reach out to me. <br />
                  </p>
                </v-col>
                <v-col cols="5">
                  <a href="mailto:priyansu.official@gmail.com" >
                  <v-btn
                    tile
                    color="#A7121D"
                    dark
                    class="mt-16 "
                    >Contact</v-btn
                  >
                </a>
                
                </v-col>
              </v-row>
            </div>
          </div>
          <v-toolbar class="topToolbar" color="#111111" dark flat>
            <div
              style="
                position: absolute;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
            >
              <v-btn text>Home</v-btn>
              <v-btn text>Project</v-btn>
              <v-btn text>About</v-btn>
              <v-btn text>Contact</v-btn>
            </div>
          </v-toolbar>
        </v-col>
      </v-row>
    </v-container>
    <FooterComponent />
  </v-app>
</template>

<script>
import NavbarComponent from "../components/NavbarComponent.vue";
import FooterComponent from "../components/FooterComponent.vue";
export default {
  name: "HomeView",

  components: {
    NavbarComponent,
    FooterComponent,
  },
  data() {
    return {
      aboutMeDialog: false,
      designDialog: false,
      frontendDialog: false,
      backendDialog: false,
    };
  },
  
};
</script>
<style scoped>
.top {
  margin-top: 180px;
}
.topInverse {
  margin-top: -250px;
}
.topToolbar {
  margin-top: 100px;
  text-align: center;
}
.first {
  width: 100%;
  height: 610px;
  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%
  );
  text-align: center;
  padding: 2rem 2rem;
}
.second {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}
.secondChild1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}

.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}
.bgColor1 {
  background-color: #1e1e1e;
}
.bgColor2 {
  background-color: #ce1d2a;
}
.child1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}
.child2 {
  display: inline-block;
  width: 245px;
  vertical-align: middle;
}
.mRight {
  margin-right: 8px;
}
.mButton {
  margin-bottom: 8px;
}
.padding {
  padding: 8px 0px;
}
.col-12.padd {
  padding: 12px 0 !important;
}
.col-12.childcol {
  padding: 0 !important;
}
h1.number {
  font-size: 50px;
  font-weight: bold;
}
.def-font-size {
  font-size: 18px;
  font-weight: 500;
}
</style>
