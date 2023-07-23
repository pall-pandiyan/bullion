(function($) {
	
	"use strict";
	var team_carousel_js = function($scope, $) {
		
		// three-item-carousel
		if ($('.four-item-carousel').length) {
			var slider_attr = $('#team-slider').data('slider');
			$('.four-item-carousel').owlCarousel({
				autoplay:slider_attr.autoplay,
				loop:slider_attr.infinite,
				margin:slider_attr.item_gap,
				nav: slider_attr.arrows,
				dots: slider_attr.dots,
				dotsEach: true,
				autoplaySpeed: slider_attr.autoplaySpeed,
				infinite: slider_attr.infinite,
				smartSpeed: 500,
				navText: [ '<span class="flaticon-left-arrow"></span>', '<span class="flaticon-right-arrow"></span>' ],
				responsive:{
					0:{
						items:1
					},
					480:{
						items:1
					},
					600:{
						items:2
					},
					800:{
						items:3
					},			
					1200:{
						items:slider_attr.item_show
					}
	
				}
			});    		
		}			
				
	};
	
	$(window).on('elementor/frontend/init', function () {
            elementorFrontend.hooks.addAction('frontend/element_ready/bullion_bullion_team_carousel.default', team_carousel_js);
    });	
	

})(window.jQuery);