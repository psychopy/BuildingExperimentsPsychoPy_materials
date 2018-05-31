A gaze cuing task
===============================================

Gaze cueing is a derivative of the Posner cuing task but, instead of having cue
that is "informative" (i.e. that is correct more often than incorrect) this
task measures your inherent tendency to follow a pair of eyes or other salient
feature even when it gives no accurate information (it is wrong as often as it
is right).

Solution
--------------

To change your Posner cueing task to this you need to:

  - fetch an image stimulus that represents a pair of eyes looking left/right
    (we've used a pair of photographic images but there are other options)
  - tweak your conditions file so that it has equal numbers of valid and invalid
    cues (we've ended up with 8 conditions rather than 10 to make this possible)
  - change your column cueOri to be called cueImage and set that to be your
    eyesRight.jpg and eyesLeft.jpg image files (or whatever yours are called)
  - change the cue in your experiment to be an Image and point this to your
    variable $cueImage. The way we've set it up here is that we've set the
    image to load during the ISI routine by creating a Static Component and
    setting the cueImage to update in that Static Period (see Chapter 12 for
    more information about static periods). This gives the most precise timing
    because otherwise the image will be loaded at the same time that PsychoPy
    tries to present it and delays will occur.

References
--------------

Posner, M.I. (1980). "Orienting of attention". Quarterly Journal of Experimental Psychology. 32 (1): 3–25.
Peirce, J.W. and MacAskill, M. (2018). "Building experiments in PsychoPy." Sage Publishing.
