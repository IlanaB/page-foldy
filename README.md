Page Foldy
==========

a SASS mixin using CSS3 for adding a fold effect to an element



INSTRUCTIONS:

1) Add foldy.scss to the folder your SASS files are in

2) Import foldy at the top of your .scss stylesheet
	* ie: in style.scss, '@import "foldy";'

3) Apply the fold to an element
	* ie:
		div{
			@include foldy({time}, {width}, {height}, {color}, {fold size}, {start position}, {shadow});
		}

4) Arguments:
* time: this sets the transition time for the fold effect
* width: sets the width of the element
* height: sets the height of the element
* color: sets the color of the element
* fold size: sets the size of the fold as a fraction of the size of the shortest side of the box (use a decimal here)
* start position: this is a guess-and-check value. IMPORTANT: based on the size of the element and the fold size this percentage will change. For a perfect square with a fold of 0.2, the start position will be 80%.
* shadow: this is either a 1 or 0 (as in true/false), indicating whether the fold is using a flat design or a more rounded, 3D effect.
