<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />

    <!-- Bootstrap CSS -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC"
      crossorigin="anonymous"
    />
    <!-- font awesome cdn -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
      integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
      crossorigin="anonymous"
      referrerpolicy="no-referrer"
    />
    <!-- style csss -->
    <link rel="stylesheet" href="style.css" />
    <!--  -->
    <script src="https://code.jquery.com/jquery-3.6.4.min.js"></script>
    <!-- Link Swiper's CSS -->
    <link
      rel="stylesheet"
      href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"
    />

    <title>Zain Cafe</title>
  </head>
  <style>
    /* swiper */
    html,
    body {
      position: relative;
      height: 100%;
    }

    .swiper {
      margin-bottom: 10px;
      z-index: -1;
    }

    .swiper-slide {
      text-align: center;
      font-size: 18px;
      background: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .swiper-slide img {
      display: block;
      width: 100%;
      height: 55vh;
      object-fit: cover;
    }

  </style>
  <body>
    <!-- navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-white">
      <div class="container-fluid mx-4">
        <a class="navbar-brand" href="/">
          <img src="./assets/images/logo.png" style="width: 4rem;height: 5rem;" alt="" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <div class="dropdown nav-link">
                <button class="dropbtn">
                  Menu <i class="fas fa-caret-down"></i>
                </button>
                <div class="dropdown-content">
                  <a href="./breakfast.html">Breakfast</a>
                  <a href="./lunch.html">Lunch</a>
                  <a href="./dinner.html">Dinner</a>
                  <a href="./fullmenu.html">Full Menu</a>
                </div>
              </div>
            </li>
            <li class="nav-item">
              <div class="nav-link dropdown">
                <button class="dropbtn">
                  About <i class="fas fa-caret-down"></i>
                </button>
                <div class="dropdown-content">
                  <a href="./ourname.html">Our Name</a>
                  <a href="./ourmission.html">Our Vision & Mission</a>
                  <a href="./contact.html">Contact</a>
                </div>
              </div>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="./login.html"> Login </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <!-- main page -->

    <!-- Swiper -->
    <div class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="./assets/images/swiper1.jpeg" alt="" />
        </div>
        <div class="swiper-slide">
          <img src="./assets/images/swiper1.jpeg" alt="" />
        </div>
        <div class="swiper-slide">
          <img src="./assets/images/swiper1.jpeg" alt="" />
        </div>
        <div class="swiper-slide">
          <img src="./assets/images/swiper1.jpeg" alt="" />
        </div>
      </div>
    </div>

    <div class="mx-3">
      <div class="row mb-3">
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/1.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Chicken Sandwich</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(1)"
              >
                <div class="">Price: $8.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-1">
                <p>Grilled chicken with lettuce, mayo and barbecue sauce.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/2.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Goat Stomach</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(2)"
              >
                <div class="">Price: $22.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-2">
                <p>
                  Grilled goat stomach served with either basmati rice or pasta
                  or chapatti.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/3.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Ugali corn meal with beef suqaar</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(3)"
              >
                <div class="">Price: $18.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-3">
                <p>Ugali corn meal served with chicken/beef suqaar.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/4.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Canbuulo Galey (Black-eye beans and sweet corn)</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(4)"
              >
                <div class="">Price: $10.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-4">
                <p>Black-eyed beans and fresh sweet corn with Juba sauce.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row mb-3">
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/5.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Shuwama Wrap</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(5)"
              >
                <div class="">Price: $12.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-5">
                <p>
                  Shuwama beef or chicken or fish served with lettuce, mayo and
                  barbecue sauce
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/6.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Goat meat</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(6)"
              >
                <div class="">Price: $25.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-6">
                <p>
                  Grilled goat meat served with basmati rice or pasta or chapati
                  flatbread.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/7.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Beef Steak</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(7)"
              >
                <div class="">Price: $18.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-7">
                <p>
                  Pasta/rice served with your choice of grilled beef/chicken
                  steak or salmon.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/8.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Chicken Steak</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(8)"
              >
                <div class="">Price: $18.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-8">
                <p>
                  Grilled chicken steak served with your choice of rice or
                  pasta.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row mb-3">
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/9.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Lamb</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(9)"
              >
                <div class="">Price: $25.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-9">
                <p>Grilled lamb shanks served with rice or pasta.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/10.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Salmon</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(10)"
              >
                <div class="">Price: $18.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-10">
                <p>Grilled salmon served with rice or pasta.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/11.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Chicken Suqaar</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(11)"
              >
                <div class="">Price: $17.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-11">
                <p>
                  Grilled chicken suqaar served with rice/past or chapati
                  flatbread.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/12.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Goat Liver</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(12)"
              >
                <div class="">Price: $12.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-12">
                <p>
                  Grilled goat liver served with Somali injera or Malawah bread.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row justify-content-center mb-3">
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/13.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Kidney Suqaar</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(13)"
              >
                <div class="">Price: $12.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-13">
                <p>
                  Grilled goat kidney served with Somali injera or Malawah
                  bread.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/14.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Beef Suqaar</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(14)"
              >
                <div class="">Price: $18.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-14">
                <p>Grilled beef suqaar served with Somali injera or Malawah.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/15.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Beef Suqaar</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(14)"
              >
                <div class="">Price: $18.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-14">
                <p>
                  Grilled beef suqaar served with rice or pasta or chapati
                  flatbread.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/16.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Spinach</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(14)"
              >
                <div class="">Price: $8.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-14">
                <p>
                  Spinach cooked with vegetables.

                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row justify-content-center mb-3">
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/17.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Bean Dip</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(13)"
              >
                <div class="">Price: $12.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-13">
                Bean and vegetables served with Somali injera or Malawah.

                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="bg-light card">
            <img src="./assets/images/18.jpeg" class="w-100" alt="" />
            <div class="card-body">
              <h5 class="">Injera with Chicken Suqaar</h5>

              <div
                class="d-flex justify-content-between"
                onclick="toggleContent(14)"
              >
                <div class="">Price: $22.00</div>
                <div class="detailsIcon"><i class="fas fa-angle-down"></i></div>
              </div>

              <div class="details-content" id="details-content-14">
                <p>
                  Ethiopian Injera served with your choice of chicken/beef suqaar, spinach, lentils and berbera hotsauce.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!--  Bootstrap JS -->
    <script
      src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js"
      integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM"
      crossorigin="anonymous"
    ></script>

    //
    <!-- Swiper JS -->
    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <!-- js code  -->
    <script>
      document.addEventListener("DOMContentLoaded", function () {
        // Hide the paragraphs on page load
        var detailsContents = document.querySelectorAll(".details-content");
        detailsContents.forEach(function (content) {
          content.style.maxHeight = "0";
        });
      });

      function toggleContent(cardId) {
        var detailsContent = document.getElementById(
          "details-content-" + cardId
        );
        var icon = document.querySelector(
          "#details-content-" + cardId + " .detailsIcon i"
        );

        if (
          detailsContent.style.maxHeight === "0px" ||
          detailsContent.style.maxHeight === ""
        ) {
          detailsContent.style.maxHeight = detailsContent.scrollHeight + "px";
          icon.classList.replace("fa-angle-down", "fa-angle-up");
        } else {
          detailsContent.style.maxHeight = "0";
          icon.classList.replace("fa-angle-up", "fa-angle-down");
        }
      }
    </script>

    <!-- Initialize Swiper -->
    <script>
      var swiper = new Swiper(".mySwiper", {
        spaceBetween: 30,
        centeredSlides: true,
        autoplay: {
          delay: 2500,
          disableOnInteraction: false,
        },
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      });
    </script>
  </body>
</html>
