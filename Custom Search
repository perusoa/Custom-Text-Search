/* Real Time Search For FAQs */
  	$("#search").keyup(function(){
			// Retrieve the input field text and reset the count to zero
			var filter = $(this).val();
			console.log(filter);
			// Loop through the comment list
			$(".faq-single").each(function(){

				// If the list item does not contain the text phrase fade it out
				if ($(this).text().search(new RegExp(filter, "i")) < 0) {
					$(this).addClass('hidden');
					$(this).removeClass('notHidden');
					if ($(this).siblings('.faq-single:not(.hidden)').length == 0) {
						$(this).closest('.faqs').parents('.faq-row').addClass('hidden');
					}
					if ($(this).siblings('.faq-single:not(.hidden)').length > 0) {
						$(this).closest('.faqs').parents('.faq-row').removeClass('hidden');
					}
				// Show the list item if the phrase matches and increase the count by 1
				} else {
					$(this).removeClass('hidden');
					$(this).addClass('notHidden');
					if ($(this).siblings('.faq-single:not(.hidden)').length == 0) {
						$(this).closest('.faqs').parents('.faq-row').addClass('hidden');
					}
					if ($(this).siblings('.faq-single:not(.hidden)').length > 0) {
						$(this).closest('.faqs').parents('.faq-row').removeClass('hidden');
					}
				}
			});
		});
