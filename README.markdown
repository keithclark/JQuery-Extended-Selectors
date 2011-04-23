#jQuery Extra Selectors#

This jQuery "plugin" adds support for the following CSS3 pseudo-class selectors to jQuery:

* :first-of-type
* :last-of-type
* :only-of-type
* :nth-of-type
* :nth-last-of-type

The project was written to service the needs of **selectivizr** users but it can be used in any project based on the jQuery library.


##Using the script##

Before using the script you'll need to include it in your page (shown below). Make sure you add it **after** the main jQuery script. Once included, you'll be able to use the selectors above in your jQuery statements.

	<script src="{path}/jquery.js"></script>
	<script src="{path}/jquery-extended-selectors.js"></script>

###Examples###

	$("div:only-of-type").css("background", "red");
	$("p:first-of-type").css("color", "red");


##Note for selectivizr users##

If you are using this script purely to extend jQuery's support for selectivizr then you'll only need to include this script for IE6-8. The best way to do that is, add it to the same conditional comment as the selectivizr script. This will prevent browsers that already support these selectors from downloading this plugin.