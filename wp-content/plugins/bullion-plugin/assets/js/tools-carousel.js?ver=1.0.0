(function($) {
	
	"use strict";
	var tool_carousel_js = function($scope, $) {
		
		var design_one = $('.tools-carousel'); 
        if(design_one.length){
            var slider_attr = $('#yt-tools-slider').data('slider');
            $('.tools-carousel').owlCarousel({
                autoplay:slider_attr.autoplay,
                loop:slider_attr.infinite,
                margin:slider_attr.item_gap,
                nav: slider_attr.arrows,
                dots: slider_attr.dots,
                dotsEach: true,
                autoplaySpeed: slider_attr.autoplaySpeed,
                infinite: slider_attr.infinite,
				navText: [ '<span class="flaticon-left-arrow"></span>', '<span class="flaticon-right-arrow"></span>' ],
                responsive:{
					0:{
						items:1
					},
					480:{
						items:1
					},
					600:{
						items:1
					},
					800:{
						items:1
					},
					1200:{
						items:slider_attr.item_show
					}
				}
            });
        }
		
	};
	$(window).on('elementor/frontend/init', function () {
            elementorFrontend.hooks.addAction('frontend/element_ready/bullion_tools_carousel.default', tool_carousel_js);
    });	

})(window.jQuery);