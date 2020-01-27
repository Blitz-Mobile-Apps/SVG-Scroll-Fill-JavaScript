# SVG-Scroll-Fill-JavaScript
Simple demonstration of filling an SVG with scroll progress for a nice and intuitive User Experience.


            SVG Fill on Scroll (Stroke filling)

    Steps:

              *HTML and CSS*
    1.  Get an SVG with path attribute. (show our SVG image here)
    2.  Wrap SVG in div, let’s say “svgDiv”.
    3.  Wrap svgDiv in another div, let’s say parent div
        and give it some height to get a vertical scroll.
    4.  Set stroke, fill, stroke-width and id on the svg.
    5.  Set the position attribute on svgDiv to fixed, so that it always stays on the center of screen.

              *JavaScript*              
    1.  Get length of the svg.
    2.  Assign strokeDashArray and strokeDashOffset to
        svg through code. The most important part as it is
        responsible for the filling of stroke in SVG.
    3. Add event listener to window scroll, and find the scrollpercentage (done through JS code snippet),
       set the offset equal to:
                    offset = pathLength – scrollpercentage
    4. Gradually the offset decreases from pathlength to 0, giving a fill effect.


        Congrats! You have hopefully learnt how to fill svg on scroll.
