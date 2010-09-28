SlideNote: A jQuery plugin for flexible, customizable sliding notifications.

HOW TO USE

1.	Include SlideNote in the header of your page. Make sure it is included after
	jQuery
	
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.4.2/jquery.min.js" type="text/javascript"></script>
	<script src="jquery.slidenote.js" type="text/javascript"></script>
	
2.	Apply the plugin to a single or set of elements.

	$('#myNote').slideNote();	// single element
	$('.notes').slideNote();	// set of elements

3. 	Pass options to the slideNote() function to modify the behavior:

	$('#myNote').slideNote({	
		where: 640,
		corner: 'left',
		url: 'ajax.html',
		container: 'note',
		closeImage: '/images/close.png'
	});
	
OPTIONS

where 			specified how far down the user must scroll before the notification
						slides into view
		
corner			controls from which side of the screen the notification will slide in

URL					tells SlideNote from where to pull the data to use as the content of
						the notification. if no container is specified, the entire page is used
		
container		to be used in conjunction with 'URL.' when specified, only pulls
						the element having the specified ID from the specified URL.
					
closeImage	if specified, will display an image that can be used to close the
						notification. once closed, the notification will not display again
						until the user has scrolled passed the where value once more.

CONTACT ME

Website: http://tommcfarlin.com
Email:	 tom@slidenote.info