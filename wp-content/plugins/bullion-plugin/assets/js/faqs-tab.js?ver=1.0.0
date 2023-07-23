(function($) {
	
	"use strict";
	var faqs_carousel_js = function($scope, $) {
		
		//Product Tabs
		if($('.faq-page-section').length){
			$('.faq-page-section .faq-tab-btns .faq-tab-btn').on('click', function(e) {
				e.preventDefault();
				var target = $($(this).attr('data-tab'));
				
				if ($(target).hasClass('actve-tab')){
					return false;
				}else{
					$('.faq-page-section .faq-tab-btns .faq-tab-btn').removeClass('active-btn');
					$(this).addClass('active-btn');
					$('.faq-page-section .faq-content .faq-tabs-content').removeClass('active-tab');
					$(target).addClass('active-tab');
				}
			});
		}
		
	
		//Accordion Box
		if($('.accordion-box').length){
			$(".accordion-box").on('click', '.acc-btn', function() {
				
				var outerBox = $(this).parents('.accordion-box');
				var target = $(this).parents('.accordion');
				
				if($(this).hasClass('active')!==true){
					$(outerBox).find('.accordion .acc-btn').removeClass('active');
				}
				
				if ($(this).next('.acc-content').is(':visible')){
					return false;
				}else{
					$(this).addClass('active');
					$(outerBox).children('.accordion').removeClass('active-block');
					$(outerBox).find('.accordion').children('.acc-content').slideUp(300);
					target.addClass('active-block');
					$(this).next('.acc-content').slideDown(300);	
				}
			});	
		}
		
	};
	$(window).on('elementor/frontend/init', function () {
            elementorFrontend.hooks.addAction('frontend/element_ready/bullion_bullion_faqs.default', faqs_carousel_js);
    });	

})(window.jQuery);