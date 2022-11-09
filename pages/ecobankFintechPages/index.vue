<template>
  <main class="main_container">
    <section class="sub_container">
      <div class="all_content">
        <!-- FIRST SECTION CONTAINER -->
        <section class="first_section_container">
          <div class="first_section_sub_container">
            <div class="large_screen_container">
              <div class="inner_content">
                <div class="logo_container">
                  <img src="../../assets/eccobamk/Green4D.png" alt="" />
                </div>
                <div class="links_container">
                  <nav>
                    <ul>
                      <li class="home_link"><a href="#">Home</a></li>
                      <li><a href="#">About</a></li>
                      <li><a href="#">transforma</a></li>
                      <li><a href="#">Partners</a></li>
                      <li class="register_btn"><button>Register</button></li>
                      <li><a href="#">Login</a></li>
                    </ul>
                  </nav>
                </div>
              </div>
            </div>
            <!-- MOBILE SCREEN -->
            <div class="mobile_screen_container">
              <div class="main_wrap">
                <div class="mobile_btn_container">
                  <button
                    class="sidebar_toggle font_btn"
                    @click="toggleSidebar"
                  >
                    <i class="fa-solid fa-bars"></i>
                  </button>
                  <button class="mobile_register_btn">Register</button>
                </div>
                <div class="mobile_screen_links" v-if="showSidebar">
                  <div class="logo_wrap">
                    <div class="mobile-logo">
                      <img src="../../assets/eccobamk/Green4D.png" alt="logo" />
                    </div>
                    <button @click="toggleSidebar" class="close_btn font_btn">
                      <i class="fa-solid fa-xmark"></i>
                    </button>
                  </div>
                  <ul class="mobile_links">
                    <li class="mobile_home_link">
                      <a href="#">Home</a>
                    </li>
                    <li>
                      <a href="#">About</a>
                    </li>
                    <li>
                      <a href="#">transforma</a>
                    </li>
                    <li>
                      <a href="#">Partners</a>
                    </li>
                    <li><a href="#">Login</a></li>
                  </ul>
                </div>
              </div>
            </div>
             <div class="card_container">
              <div class="card_content">
                <div class="card_header">
                  <h1>4D Digital Green Corridor</h1>
                </div>
                <div class="card_paragraph">
                  <p>
                    An initiative of the African Union and it's partners to
                    drive the adoption of climate-smart and ecological sound
                    technologies by Africa's industrial operators, and thus
                    create green jobs in urban corridors for the continent's
                    teeming youth.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </section>
        <!--END OF FIRST SECTION CONTAINER -->
        <!-- SECOND SECTION CONTAINER -->
        <section class="second_section_container">
          <div class="second_section_sub_container">
           

            <div class="about_container">
              <div class="about_sub_container">
                <div class="about_header">
                  <h1>What you need to know</h1>
                </div>
                <div class="about_content">
                  <div class="about_first_para">
                    <p>
                      The 4D Digital Green Corridor is a "multistakeholder
                      innovation" concept promoted by the African Union and its
                      partners and organs; major governments; green tech
                      industries; AfroChampions; and many leading technology
                      innovators and accelerators.
                    </p>
                  </div>
                  <div class="about_second_para">
                    <p>
                      It connects and deepens the value chains that will power
                      Africa's industrialisation through climate-smart
                      technology transfer, creating vast numbers of jobs
                      eventually for Africa's teeming youth.
                    </p>
                  </div>
                  <div class="about_third_para">
                    <p>
                      Leveraging major forces like AfCFTA and the Green Recovery
                      Action Plan for Africa (GRAP), it is removing barriers and
                      obstacles in the way of smart trade in Africa and
                      accelerating the circulation of the talents and skills
                      that will boost African integration for continental
                      transformation.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <!-- END OF SECOND SECTION CONTAINER-->
        <!-- THIRD SECTION CONTAINER-->
        <section>
          <transforma />
        </section>
        <!-- END OF THIRD SECTION CONTAINER-->
      

        
      </div>
    </section>
  </main>
</template>

<script>
import transforma from "../../components/ecobankFintech/transforma.vue"
// import Partners from '../../components/ecobankFintech/partners.vue'
export default {
  components: { transforma},
  data() {
    return {
      showSidebar: false,
    };
  },
  methods: {
    toggleSidebar() {
      this.showSidebar = !this.showSidebar;
    },
  },
};
</script>

<style scoped>
.main_container {
  width: 100%;
  height: 100vh;
}

/* FIRST SECTION CONTAINER */
.first_section_container {
  width: 100%;
  height: 100%;
}

.first_section_sub_container {
  width: 100%;
  height: 800px;
  background: linear-gradient(
      227.86deg,
      rgba(0, 72, 70, 0.8) 0%,
      rgb(0, 218, 122, 0.8) 100%
    ),
    url("../../assets/eccobamk/Rectangle2.png") center;
  background-size: cover;
}

.inner_content {
  display: flex;
  justify-content: space-between;
  align-items: space-between;
  padding-top: 100px;
  padding-left: 200px;
  padding-right: 200px;
}

.logo_container img {
  width: 250px;
  height: 50px;
  object-fit: cover;
  display: block;
}

.links_container nav ul {
  display: flex;
  justify-content: space-between;
  align-items: space-between;
  gap: 20px;
}

.links_container nav ul li {
  list-style-type: none;
}
.links_container nav ul li a {
  text-decoration: none;
}

.links_container nav ul li:not(.home_link) a {
  font-family: "Montserrat-bold";
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 17px;
  color: #ffffff;
  cursor: pointer;
}

.links_container nav ul .home_link a {
  font-family: "Montserrat-bold";
  font-style: normal;
  font-weight: 800;
  font-size: 14px;
  line-height: 17px;
  color: #00da7a;
  cursor: pointer;
}

.links_container nav ul .register_btn button,
.mobile_screen_container .mobile_register_btn {
  width: 78px;
  height: 38px;
  background: #00da7a;
  border-radius: 26px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 17px;
  color: #004846;
  border: none;
  outline: none;
  cursor: pointer;
}

/* Mobile Screen Container*/

/*End Of  Mobile Screen Container*/
.mobile_btn_container {
  display: flex;
  justify-content: space-between;
  align-items: space-between;
  padding: 30px;
}

.mobile_screen_container .sidebar_toggle {
  font-size: 30px;
  border: none;
  color: #00da7a;
  width: 50px;
  height: 50px;
  border-radius: 10px;
  background-color: transparent;
  transition: all 0.3s linear;
}

.mobile_screen_container .sidebar_toggle:hover,
.close_btn:hover {
  border: 1px solid #004846;
}

.mobile_screen_links {
  background-color: #868181;
  width: 100%;
  height: 500px;
  position: fixed;
  top: 0;
  transform: translateX(0%);
  z-index: 5;
}

.showSlide {
  transform: translateX(0);
}

.logo_wrap {
  display: flex;
  justify-content: space-between;
  align-items: space-between;
  padding: 2rem;
}

.mobile-logo img {
  width: 250px;
  height: 50px;
  object-fit: cover;
  display: block;
}

.logo_wrap .close_btn {
  font-size: 30px;
  border: none;
  background-color: transparent;
  color: #fff;
}

.mobile_links li {
  list-style-type: none;
  margin-top: 15px;
}

.mobile_links li a {
  text-decoration: none;
}

.mobile_links .mobile_home_link a {
  font-family: "Montserrat-bold";
  font-style: normal;
  font-weight: 800;
  font-size: 25px;
  line-height: 17px;
  color: #00da7a;
  cursor: pointer;
}
.mobile_links li:not(.mobile_home_link) a {
  font-family: "Montserrat-bold";
  font-style: normal;
  font-weight: 300;
  font-size: 25px;
  line-height: 17px;
  color: #000000;
  cursor: pointer;
}

/*END OF FIRST SECTION CONTAINER */

/*SECOND SECTION CONTAINER */
.second_section_container {
  width: 100%;
  height: 100%;
}

.second_section_sub_container {
  height: 500px;
  background-color: #ffffff;
}

.card_container {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  top: 350px;
}

/*Card Container */

.card_content {
  width: 100%;
  height: 100%;
  max-width: 1170px;
  max-height: 643px;
  background: linear-gradient(227.86deg, #004846 0%, #00da7a 100%);
  border-radius: 30px;
  z-index: 1;
}
.card_container .card_header {
  width: 438px;
  height: 120px;
  margin: 80px auto 0 auto;
}

.card_container .card_header h1 {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 800;
  font-size: 64px;
  line-height: 60px;
  text-align: center;
  color: #ffffff;
}

.card_container .card_paragraph {
  width: 624px;
  height: 104px;
  margin: 80px auto 100px auto;
}

.card_container .card_paragraph p {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 24px;
  text-align: center;
  color: #ffffff;
}

/* End Of Card Container */

/*About Container */

.about_container {
  margin-top: 200px;

}

.about_content {
  width: 100%;
  height: 100%;
  max-width: 824px;
  max-height: 312px;
  margin: 62px auto 0px auto;
}

.about_container p {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 24px;
  text-align: center;
  color: #004846;
  margin-top: 30px;
  padding-left: 10px;
  padding-right: 10px;
}

.about_container .about_header h1 {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 800;
  font-size: 32px;
  line-height: 39px;
  text-align: center;
  color: #009160;
}
/*End Of Card Container */

/*END OF SECOND SECTION CONTAINER */

/* MEDIA QUERIES */
@media screen and (max-width: 2560px) {
  .large_screen_container {
    display: block;
  }
  .mobile_screen_container {
    display: none;
  }
}
@media screen and (max-width: 1300px) {
  .inner_content {
    padding-left: 100px;
    padding-right: 100px;
  }
}

@media screen and (max-width: 900px) {
  .logo_container {
    display: none;
  }
}
@media screen and (max-width: 600px) {
  .large_screen_container {
    display: none;
  }
  .mobile_screen_container {
    display: block;
  }

  .card_container .card_header {
    width: 350px;
  }
  .card_container .card_header h1 {
    font-size: 40px;
  }

  .card_container .card_paragraph {
    width: 350px;
  }
}
</style>
