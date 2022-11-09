<template>
  <main class="main_container">
    <section class="sub_container">
      <div class="all_content">
        <!-- TRANSFORMA CONTAINER -->
        <section class="transforma_container">
          <div class="transforma_sub_container">
            <div class="header_container">
              <div class="transforma_logo_wrap">
                <img src="../../assets/eccobamk/Vector (2).svg" alt="" />
              </div>
              <div class="transforma_header_text">
                <h1>transforma</h1>
                <h3>Powered By <span>Green4D</span></h3>
              </div>
            </div>
            <div class="overview_container">
              <div class="overview_sub_container">
                <div class="overview_left_text_wrap">
                  <div class="overview_text_header">
                    <h1>Overview</h1>
                  </div>
                  <div class="overview_content_para">
                    <div class="overview_first_para">
                      <p>
                        The opportunities to use natural gas as an economic
                        policy means to resolve unproductive tensions between
                        the climate innovation agenda and the urgent need to
                        overcome energy poverty in Africa is well understood and
                        widely discussed.
                      </p>
                    </div>
                    <div class="overview_second_para">
                      <p>
                        But with three quarters of Africa's population still
                        being denied participation in the emerging clean energy
                        sector, whether as consumers, skilled workers or
                        producers, the current policy innovations to bridge the
                        gap between the various energy and climate camps appear
                        too few and too slow.
                      </p>
                    </div>
                    <div class="overview_third_para">
                      <p>
                        The African Union and its strategic partner,
                        AfroChampions, have thus joined forces with pioneering
                        governments around Africa and private sector enablers to
                        create a model multi-stakeholder innovation platform to
                        show the recent advances in practices.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="transforma_right_text_wrap">
                  <div class="transforma_text_header">
                    <h1>Why Transforma?</h1>
                  </div>
                  <div class="transforma_content_para">
                    <div class="transforma_first_para">
                      <p>
                        As a supranational and multistakeholder accelerator,
                        Transforma will focus, as a first step, on modular
                        natural gas liquids at the meso-scale with an emphasis
                        on supply chain transformation.
                      </p>
                    </div>
                    <div class="transforma_second_para">
                      <p>
                        Through creative network solutions, the collaborators
                        intend to cut the costs of equitable access, reinforce
                        safety, enhance economic circularity, boost regulatory
                        capacity for quality assurance and firm up climate
                        impact auditing at all levels. The initial slate of
                        government partners come from the AfCFTA Guided Trade
                        Initiative stable.
                      </p>
                    </div>
                    <div class="transforma_third_para">
                      <p>
                        These partner agencies have committed resources to
                        underwrite significant risks for major private sector
                        partners to innovate their supply chain infrastructure
                        and practices to meet the unmet needs of medium-scale
                        enterprises, housing complexes and other consumers
                        critical to Africa’s value addition targets in line with
                        Agenda 2063 and the 4D framework.
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="large_logo_container">
              <div class="large_logo_sub_container">
                <div class="logo_img">
                  <img
                    src="../../assets/eccobamk/trasforma pattern (1).png"
                    alt=""
                  />
                  <div class="petrol_img">
                    <img
                      class="petrol_img"
                      src="../../assets/eccobamk/petrol image.png"
                      alt=""
                    />
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <!--END OF TRANSFORMA CONTAINER -->
          <!-- PARTNERS IMAGE CONTAINER -->
        <section>
          <Partners />
        </section>
        <!-- END OF PARTNERS IMAGE CONTAINER-->
      </div>
    </section>
  </main>
</template>

<script>
import Partners from './partners.vue'
export default {
  components: {Partners}
};
</script>

<style scoped>
.main_container {
  width: 100%;
  height: 100vh;
}

.transforma_container {
  width: 100%;
  height: 100%;
  background: #004846;
}

.header_container {
  padding-top: 150px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 70px;
}

.header_container .transforma_logo_wrap img {
  width: 100%;
  height: 100%;
  max-width: 268px;
  max-height: 245px;
  object-fit: cover;
  display: block;
}

.transforma_header_text h1 {
  color: #ffffff;
  font-family: "Montserrat-bold";
  font-style: normal;
  font-weight: 800;
  font-size: 100px;
  line-height: 17px;
  margin-bottom: 40px;
}

.transforma_header_text h3 {
  font-family: "Montserrat-bold";
  font-style: normal;
  font-weight: 300;
  font-size: 24px;
  line-height: 17px;
  color: #ffffff;
}

.transforma_header_text span {
  color: #00da7a;
}

/*Overview Container */
.overview_sub_container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  gap: 30px;
  margin-top: 100px;
}
.overview_container .overview_text_header h1,
.transforma_text_header h1 {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 800;
  font-size: 32px;
  line-height: 39px;
  color: #00da7a;
}
.overview_container .overview_content_para,
.transforma_content_para {
  width: 570px;
  height: 468px;
  padding-bottom: 10px;
}

.overview_content_para p,
.transforma_content_para {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 24px;
  color: #ffffff;
}

/* Large Logo Container */
.logo_img {
  position: relative;
  padding-bottom: 40px;
}
.large_logo_container .logo_img img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.petrol_img img {
  position: absolute;
  top: 80px;
  right: 200px;
  width: 100%;
  height: 100%;
  max-width: 1100px;
  max-height: 618px;
}
/* End Of Large Logo Container */

/* MEDIA QUERIES*/
@media screen and (min-width: 700px) {
  .petrol_img img {
    top: 40px;
    right: 60px;
    max-width: 600px;
  }
}
@media screen and (min-width: 1000px) {
  .petrol_img img {
    right: 100px;
    max-width: 800px;
  }
}

@media screen and (min-width: 1200px) {
  .petrol_img img {
    position: absolute;
    top: 70px;
    right: 200px;
    max-width: 1100px;
    max-height: 618px;
  }
}

@media screen and (min-width: 2000px) {
  .petrol_img img {
    max-width: 1500px;
    max-height: 700px;
    top: 320px;
    right: 400px;
  }
}
@media screen and (max-width: 800px) {
  .header_container .transforma_logo_wrap img {
    width: 170px;
  }

  .transforma_header_text h1 {
    font-size: 70px;
  }
}

@media screen and (max-width: 600px) {
  .main_container {
    margin-top: 400px;
  }
  .transforma_right_text_wrap {
    margin-top: 90px;
  }
  .header_container .transforma_logo_wrap {
    display: none;
  }

  .transforma_header_text h1 {
    font-size: 70px;
  }
}

/* MEDIA QUERIES*/
@media screen and (max-width: 1300px) {
  .overview_sub_container {
    flex-direction: column;
    gap: 10px;
  }
}

@media screen and (max-width: 600px) {

.main_container {
  margin-top: 130px;
}
  .overview_container .overview_content_para,
  .transforma_content_para {
    width: 350px;
  }

  .overview_sub_container {
    flex-direction: column;
    gap: 10px;
  }

  .overview_sub_container {
    padding-bottom: 170px;
  }

  .logo_img {
    display: none;
  }
}
</style>
