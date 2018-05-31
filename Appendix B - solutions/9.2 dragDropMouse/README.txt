Change contrast with mouse hover
=======================================

You can even add a little bit of code to allow participants to move the
stimuli around using the mouse. You might want to see how they organise a series
of images on the screen for instance.

Solution
-----------------

The basis of this is just like the hover images example but we're doing a bit
more this time. You need to:

  - set the window units to be in 'pix' in Experiment Settings, because that
    determines the units of the reported mouse position. In this trial we will
    set the position of each image (which is in pixels) to match the position
    of the mouse so we need to make sure that's in pixels too!
  - set the mouse NOT to end the Routine on a click because we're wanting to
    use the click to indicate the start of a "drag" period
  - write the actual code to handle the dragging of the images. You could write
    `if mouse.isPressedIn(image_1):` but we used the slightly longer version:
    `if image_1.contains(mouse) and sum(mouse.getClicked()):` which tells you a
    bit more about the meaning of "isPressedIn". The two things are equivalent.
  - if you also want to save the final positions of your images then note also
    the code in the where we save the position as an x value and a y value for
    each image in the trial. You could save them as simply a position (x, y)
    but then it will be harder to handle in your analysis software.

References
-----------------

Peirce, J.W. and MacAskill, M. (2018). "Building experiments in PsychoPy." Sage Publishing.
