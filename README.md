# Instagram-Stick-Slider-jQuery


Description
---------------------------------------------------------------------------------------------------------------------------------------
a lightWeight responsive content slider with stick

Demo
-----------------------------------------------------------------------------------------------------------------------------------
<a href="https://140.82.58.117/tingshop/">Instagram Stick Slider</a>

Main Features
---------------------------------------------------------------------------------------------------------------------------------------
  Fully responsive - will adapt to any device.
  
  Separate settings per breakpoint.
  
  Gallery mode to create an image slideshow with thumbnails
  
  Supports swipe and mouseDrag
  
  Add or remove slides dynamically.
  
  Small file size, fully themed, simple to implement.
  
  CSS transitions with jQuery fallback.
  
  Full callback API and public methods.
  
  Auto play and infinite loop to create a content carousel.
  
  Keyboard, arrows and dots navigation. 
  
  Chrome, Safari, Firefox, Opera, IE7+, IOS, Android, windows phone.
  
The Code 
  add the following code to the <head> of your code.
  
      <link type="text/css" rel="stylesheet" href="css/lightslider.css" />
      <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
      <script src="js/lightslider.js"></script>
      // Do not include both lightslider.js and lightslider.min.js

  Slider Settings
  
    <script type="text/javascript">
      $(document).ready(function() {
          $("#light-slider").lightSlider({
              item: 3,
              autoWidth: false,
              slideMove: 1, // slidemove will be 1 if loop is true
              slideMargin: 10,

              addClass: '',
              mode: "slide",
              useCSS: true,
              cssEasing: 'ease', //'cubic-bezier(0.25, 0, 0.25, 1)',//
              easing: 'linear', //'for jquery animation',////

              speed: 400, //ms'
              auto: false,
              pauseOnHover: false,
              loop: false,
              slideEndAnimation: true,
              pause: 2000,

              keyPress: false,
              controls: true,
              prevHtml: '',
              nextHtml: '',

              rtl:false,
              adaptiveHeight:false,

              vertical:false,
              verticalHeight:500,
              vThumbWidth:100,

              thumbItem:10,
              pager: true,
              gallery: false,
              galleryMargin: 5,
              thumbMargin: 5,
              currentPagerPosition: 'middle',

              enableTouch:true,
              enableDrag:true,
              freeMove:true,
              swipeThreshold: 40,

              responsive : [],

              onBeforeStart: function (el) {},
              onSliderLoad: function (el) {},
              onBeforeSlide: function (el) {},
              onAfterSlide: function (el) {},
              onBeforeNextSlide: function (el) {},
              onBeforePrevSlide: function (el) {}
          });
      });
    </script>

Public methods

    <script type="text/javascript">
        $(document).ready(function() {
            var slider = $("#light-slider").lightSlider();
            slider.goToSlide(3);
            slider.goToPrevSlide();
            slider.goToNextSlide();
            slider.getCurrentSlideCount();
            slider.refresh();
            slider.play();
            slider.pause();
            slider.destroy();
        });
    </script>
