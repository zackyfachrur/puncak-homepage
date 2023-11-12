# 1KA02
#### Kenang - Kenangan semasa kuliah
Preview Front-End 😉 :
```js
$(document).ready(function () {
    $(".navbar .nav-link").on("click", function (event) {
      if (this.hash !== "") {
        event.preventDefault();
  
        var hash = this.hash;
  
        $("html, body").animate(
          {
            scrollTop: $(hash).offset().top,
          },
          700,
          function () {
            window.location.hash = hash;
          }
        );
      }
    });
  });
  
  $("#nav-toggle").click(function () {
    $(this).toggleClass("is-active");
    $("ul.nav").toggleClass("show");
  });
  
  document.onkeydown = function (e) {
    if (event.keyCode == 123) {
      return false;
    }
  
    if (e.ctrlKey && e.shiftKey && e.keyCode == "I".charCodeAt(0)) {
      return false;
    }
  
    if (e.ctrlKey && e.shiftKey && e.keyCode == "J".charCodeAt(0)) {
      return false;
    }
  
    if (e.ctrlKey && e.keyCode == "U".charCodeAt(0)) {
      return false;
    }
  };
  
  var swiper = new Swiper(".content", {
    slidesPerView: 3,
    spaceBetween: 20,
    grabCursor: "true",
    pagination: {
      el: ".swiper-pagination",
      clickable: true,
    },
    breakpoints: {
      0: {
        slidesPerView: 1,
      },
      520: {
        slidesPerView: 2,
      },
      950: {
        slidesPerView: 2,
      },
    },
  });
  
```
