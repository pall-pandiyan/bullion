(function($) {
	
	"use strict";
	var choose_carousel_js = function($scope, $) {
		
		// three-item-carousel
		var design_one = $('.te-three-item-carousel'); 
        if(design_one.length){
            var option_attr = $('.te-three-item-carousel').data('slider');
            $('.three-item-carousel').owlCarousel({
                autoplay:option_attr.autoplay,
                loop:option_attr.infinite,
                margin:option_attr.item_gap,
                nav: option_attr.arrows,
                dots: option_attr.dots,
                dotsEach: true,
                autoplaySpeed: option_attr.autoplaySpeed,
                infinite: option_attr.infinite,
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
						items:2
					},			
					1200:{
						items:option_attr.item_show
					}	
				}
				
            });
        }
		
	};	
	$(window).on('elementor/frontend/init', function () {
            elementorFrontend.hooks.addAction('frontend/element_ready/bullion_why_choose_us.default', choose_carousel_js);
    });	

})(window.jQuery);