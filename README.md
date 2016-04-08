= Installation =

  # Extract zip file in the modules directory
  # Enable the module in the admin settings
  # Add the filter in the input format you want to use.

= Use =

To insert a flimme frame in a node in drupal, add the following :

 [[[flimme element=<element-identifier> type=<flim|event|auth> width=<w> height=<h> className=<class> ID=<id>]]]

Note: > and < are not inserted, and a single space is required between variables.

Where
 
	element-identifier is the id, event-name or stream-name for the frame
	type is the type of the stream (single flim, event or authenticated stream) ==> Default : flim
	w is the width as css declaration (%,px,em) ==> Default : 100%
    h is the height as css declaration (%,px,em). if height=100% and url is in the same domain as web site, the height will be ajusted to the real height of the source ==> Default 100%
	class is a CSS class ==> Default : none
    ID is the id and name of the frame ==> default : iframe<no of the frame in the node (if multiple)>

Only ELEMENT-IDENTIFIER is required.

= Create Text Format For Use With Insert Frame =

Name: Flimme Frame for Drupal

Enabled Filters: Check "Include Flimme-iFrame"

Save Configuration

= Example =

Following is a properly configured, inserted flimme frame:

[[[flimme element=172047 width=98% height=500px]]]


 