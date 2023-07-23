(function($) {
	
	"use strict";
	var educations_carousel_js = function($scope, $) {
		
		// courses-tab
		if($('.courses-tab').length){
			$('.courses-tab .courses-tab-btns .p-tab-btn').on('click', function(e) {
				e.preventDefault();
				var target = $($(this).attr('data-tab'));
				
				if ($(target).hasClass('actve-tab')){
					return false;
				}else{
					$('.courses-tab .courses-tab-btns .p-tab-btn').removeClass('active-btn');
					$(this).addClass('active-btn');
					$('.courses-tab .p-tabs-content .p-tab').removeClass('active-tab');
					$(target).addClass('active-tab');
				}
			});
		}	
		
		// three-item-carousel
		var design_one = $('.course-item-carousel'); 
        if(design_one.length){
            var slider_attr = $('#education-carousel').data('slider');
            $('.course-item-carousel').owlCarousel({
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
				
	};
	
	$(window).on('elementor/frontend/init', function () {
            elementorFrontend.hooks.addAction('frontend/element_ready/bullion_courses_tab_carousel.default', educations_carousel_js);
    });	
	

})(window.jQuery);