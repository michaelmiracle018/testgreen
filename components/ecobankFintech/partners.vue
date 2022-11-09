<template>
  <main class="main_container">
    <section class="sub_container">
      <!-- PARTNERS IMAGE CONTAINER -->
      <div class="partners_container">
        <div class="partners_sub_container">
          <div class="partners_header">
            <h1>Strategic Partners</h1>
          </div>
          <div class="partners_image_container">
            <div class="partners_image_sub_container">
              <div class="first_image_content">
                <div>
                  <img
                    class="first_img"
                    src="../../assets/eccobamk/afcfta.svg"
                    alt=""
                  />
                </div>
                <div>
                  <img
                    class="second_img"
                    src="../../assets/eccobamk/7 2B 1.png"
                    alt=""
                  />
                </div>
                <div>
                  <img
                    class="third_img"
                    src="../../assets/eccobamk/auweblogo-en 1.png"
                    alt=""
                  />
                </div>
              </div>
              <div class="second_image_content">
                <div>
                  <img
                    class="fourth_img"
                    src="../../assets/eccobamk/AFROCHAMPION INITIATIVE RED  PNG 1.png"
                    alt=""
                  />
                </div>
                <div>
                  <img
                    class="fifth_img"
                    src="../../assets/eccobamk/badea 1.png"
                    alt=""
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!--END OF PARTNERS IMAGE CONTAINER -->
      <!-- FOOTER CONTAINER -->
      <footer>
        <div class="left_footer_text">
          <h2>
            All rights reserved. Copyright 4D Digital Green Corridors © 2021
          </h2>
        </div>
        <div class="right_footer_text">
          <h2>Terms & Conditions Privacy Policy</h2>
        </div>
      </footer>
      <!--END OF FOOTER CONTAINER -->
    </section>
  </main>
</template>

<script>
export default {};
</script>

<style scoped>
.main_container {
  margin-top: 50px;
  width: 100%;
  height: 100%;
}

.partners_container {
  max-width: 1520px;
  max-height: 1120px;
}

.partners_header h1 {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 800;
  font-size: 32px;
  line-height: 39px;
  text-align: center;
  color: #009160;
  margin-top: 190px;
}

.partners_container {
  width: 100%;
  height: 100%;
  margin: 0 auto;
}

.first_img {
  width: 100%;
  max-width: 250px;
  height: 150px;
  object-fit: cover;
  display: block;
}
.second_img,
.third_img,
.fourth_img,
.fifth_img {
  width: 100%;
  height: 100%;
  max-width: 300px;
  max-height: 200px;
  object-fit: cover;
  display: block;
}
.first_image_content {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  gap: 70px;
  margin-top: 150px;
}

.second_image_content {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  gap: 80px;
  margin-top: 20px;
}

footer {
  display: flex;
  justify-content: space-between;
  align-items: space-between;
  flex-direction: row;
  padding-left: 50px;
  padding-right: 50px;
  margin-top: 100px;
}

footer .left_footer_text h2,
.right_footer_text h2 {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 24px;
  text-align: center;
  color: #004846;
}

@media screen and (max-width: 900px) {
  .second_image_content {
    margin-top: 60px;
    gap: 30px;
  }

  footer {
    flex-direction: column;
    gap: 30px;
  }
}
</style>
