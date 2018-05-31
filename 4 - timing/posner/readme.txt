The Posner cuing task
===============================================

This experiment provides a simple demonstration of the Posner cuing effect in which reaction times are faster when participants are detecting a stimulus in the position that they were expecting it to appear rather than a stimulus appearing in a different location.

NB in the book we teach you to use units of degrees for this example, but here we're sticking
with pixels so that it will work even if you haven't provided calibration information to your monitor.

The task
--------------

On each trial participants must response as quickly as possible to report, using the left/right arrow keys on the keyboard, in which of two locations a "target" stimulus, in our case a green circle, appears.

Before that target, a cue directs the participant's attention to either the left or right of the screen. In the version of the task we are using (Posner and other labs have tested a huge range of similar tasks) the cue is a triangle and correctly indicates the location that the target will appear on 80% of the trials. On the remaining 20% of trials the target stimulus will appear in the other location.

Implementation notes
-------------------------

We have created a variable inter-trial interval (ITI) in this demo. The way this has been implemented, we have created a separate Routine called ITI with a fixation point that lasts for 1+random() seconds (that's a value between 1 and 2 seconds). It isn't strictly necessary to do this with a separate Routine but it's convenient because it means that we automatically shift all the Components in the main trial Routine by the same random jitter in one go. Otherwise we would need to keep track of the random jitter on each trial (with a variable) and apply it to each of the stimuli (cue, target etc.)

References
--------------

Posner, M.I. (1980). "Orienting of attention". Quarterly Journal of Experimental Psychology. 32 (1): 3–25.
Peirce, J.W. and MacAskill, M. (2018). "Building experiments in PsychoPy." Sage Publishing.
