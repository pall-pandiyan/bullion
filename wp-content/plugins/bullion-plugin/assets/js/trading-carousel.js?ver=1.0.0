(function($) {
	
	"use strict";
	var trade_carousel_js = function($scope, $) {
		
		// three-item-carousel
		var design_one = $('.trading-three-item-carousel'); 
        if(design_one.length){
            var slider_attr = $('.trading-three-item-carousel').data('slider');
            $('.trading-three-item-carousel').owlCarousel({
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
						items:2
					},
					800:{
						items:2
					},			
					1200:{
						items:slider_attr.item_show
					}	
				}
				
            });
        }
		
		// single-item-carousel
		var design_two = $('.trading-single-item-carousel'); 
        if(design_two.length){
            var option_attr = $('.trading-single-item-carousel').data('slider');
            $('.trading-single-item-carousel').owlCarousel({
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
						items:1
					},
					800:{
						items:1
					},			
					1200:{
						items:option_attr.item_show
					}
	
				}
				
            });
        }			
				
	};
	
	$(window).on('elementor/frontend/init', function () {
            elementorFrontend.hooks.addAction('frontend/element_ready/bullion_bullion_trading_carousel.default', trade_carousel_js);
    });	
	

})(window.jQuery);