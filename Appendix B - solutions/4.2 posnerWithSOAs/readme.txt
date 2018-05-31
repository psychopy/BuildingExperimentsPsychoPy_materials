The Posner cuing task with variable SOA
===============================================

This experiment tests the effect of the Stimulus Onset Asynchrony (SOA) on the effect of attentional cuing. A common finding (but you may need quite a few participants and/or trials is that very brief cues have little effect, moderat-duration cues (e.g. 200-300ms) have most positive effect and very long cues can actually make RT worse (an effect known as inhibition of return).

A data files showing exactly that pattern can be seen in the data folder here (see the file called P32_posnerSOA_analysis.xlsx)

The task
--------------

On each trial participants must response as quickly as possible to report, using the left/right arrow keys on the keyboard, in which of two locations a "target" stimulus, in our case a green circle, appears.

Before that target, a cue directs the participant's attention to either the left or right of the screen. In the version of the task we are using (Posner and other labs have tested a huge range of similar tasks) the cue is a triangle and correctly indicates the location that the target will appear on 80% of the trials. On the remaining 20% of trials the target stimulus will appear in the other location.

Implementation notes
-------------------------

The conditions file needs the following changes:
  - equal numbers of valid/invalid cues (you could now have just the 4 options of left/right valid/invalid)
  - an additional column of SOA_frames (we'll use number of screen refreshes to measure the onset asynchrony). We've used 6, 12, 24, 48 frames (100, 200, 400, and 800 ms on a 60Hz monitor)
  - the 4 valid/invalid rows need to be repeated for each of your SOA values, resulting in 16 rows of conditions

Fetch your Posner task from Chapter 4. Alter it so that:
  - the trial->cue has duration of SOA_frames
  - the trial->target has a start of SOA_frames
  - the trials loop needs to use the new conditions file (and should show 16 conditions)
  - the trials->nReps should be set to something higher so that you have more trials of each condition (e.g. 8)

Running 16 conditions 8 times each means 128 trials overall. Each trial lasts at most 4 seconds, so the experiment should take less than 9 minutes to complete, but a lot less than that for most participants with fast reaction times.

References
--------------

Posner, M.I. (1980). "Orienting of attention". Quarterly Journal of Experimental Psychology. 32 (1): 3–25.
Peirce, J.W. and MacAskill, M. (2018). "Building experiments in PsychoPy." Sage Publishing.
