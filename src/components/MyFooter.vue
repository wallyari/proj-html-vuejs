<template>
  <footer>
    <div class="container-faq d-flex">
      <div class="faq d-flex justify-content-center align-items-center">
        <div class="faq-box d-flex">
          <!-- RESTAURANT -->
          <div class="restaurants">
            <h4 class="text-uppercase">find our restaurants</h4>
            <ul v-for="(restaurant, index) in restourantArray" :key="index">
              <li>{{ restaurant.address }}</li>
              <li>{{ restaurant.city }}</li>
              <li>{{ restaurant.phoneNumber }}</li>
            </ul>
          </div>

          <!-- WORKING HOURS -->
          <div class="working-hours">
            <h4 class="text-uppercase">working hours</h4>
            <ul v-for="(info, i) in infoArray" :key="`id2-${i}`">
              <li class="day text-uppercase">
                {{ info.day }}<span v-show="info.check">*</span>
              </li>
              <li
                :class="{ shopClosed : info.workingHours == 'Kitchen Closed' }"
              >
                {{ info.workingHours }}
              </li>
            </ul>

            <ul class="socials d-flex">
              <h4 class="text-uppercase">Follow Us:</h4>
              <li>
                <a href="/"><i class="fab fa-twitter"></i></a>
              </li>
              <li>
                <a href="/"><i class="fab fa-facebook-f"></i></a>
              </li>
              <li>
                <a href="/"><i class="fab fa-instagram"></i></a>
              </li>
              <li>
                <a href="/"><i class="fab fa-linkedin-in"></i></a>
              </li>
            </ul>
          </div>

          <!-- DON PEPPE QUOTE -->
          <div class="quote text-uppercase">
            the don peppe crew <br />
            first and foremost <br />
            values an authentic,<br />
            well baked slice of <br />
            pizza.
          </div>
        </div>

        <!-- LOGO  -->
        <a href="">
          <img
            class="product-logo"
            src="../assets/img/h1-clients-img-3.png"
            alt=""
          />
        </a>

        <!-- signature -->
        <div class="signature">
          Created with &#9829; by
          <a class="sig-color" href="/">Ansia</a>
        </div>
      </div>
      <div class="bg-footer">
        <img src="../assets/img/footer-img-1.jpg" alt="" />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: " MyFooter",
  data() {
    return {
      restourantArray: [
        {
          address: "1614 E. Bell Rd #104.",
          city: "Salerno, AZ 85022",
          phoneNumber: "(602) 867-1010",
        },
        {
          address: "204 E. Pizzetta Tommaso",
          city: "Sorrento, AZ 85022",
          phoneNumber: "(358) 867-1010",
        },
        {
          address: "Vale Puglia 54",
          city: "Torre Del Greco, AZ 85022",
          phoneNumber: "(359) 867-1010",
        },
        {
          address: "Corso Itali AA",
          city: "Naples, AZ 85022",
          phoneNumber: "(989) 867-1010",
        },
      ],
      infoArray: [
        {
          day: "monday",
          workingHours: "Kitchen Closed",
          check: false,
        },
        {
          day: "tuesady until friday",
          workingHours: "9:00 - 22:00",
          check: false,
        },
        {
          day: "saturday",
          workingHours: "Saturday 11am to midnight",
          check: true,
        },
        {
          day: "sunday",
          workingHours: "9:00 - 22:00",
          check: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

footer {
  height: 600px;
  overflow: hidden;
  .container-faq {
    height: 100%;
    .faq,
    .bg-footer {
      width: 50%;
    }
    .faq {
      background-color: $bg-header;
      color: white;
      position: relative;
      padding-bottom: 55px;
      h4 {
        color: #B68A2C;
        font-weight: 500;
        letter-spacing: 1px;
      }
      .faq-box {
        justify-content: space-between;
        width: 90%;
        ul {
          list-style-type: none;
          padding-top:15px;
          font-size: 13px;
          color: white;
          font-weight: 300;
          letter-spacing: 1px;
        }
        .working-hours {
          ul {

              span {
                color: white;
                font-size:10px;
                padding-left: 10px;
              }
            }
            .day {
              color: white;
            }
          }
          .socials {
            padding-top: 30px;
            h4 {
              font-weight: 400;
              letter-spacing: 0.5px;
            }
            i {
              padding: 15px;
              font-size: 20px;
            }
          }
        }
      }
      .quote {
        width: 35%;
        font-size: 23px;
      }
      .product-logo {
        position: absolute;
        right: 5%;
        bottom: 7%;
      }
      .signature {
        position: absolute;
        bottom: 7%;
        left: 5%;
        font-size: 13px;
        color: $bg-header;
        font-weight: 300;
        letter-spacing: 1px;
        .sig-color {
          color: white;
        }
      }
    }
    .bg-footer {
    width: 50%;
    img {
    width: 100%;

    }
}
  }

// per passaggio
.shopClosed {
  color: white;
}
</style>