Stroop task, with feedback included
============================================================

The experiment
------------------------

This extends the basic Stroop task that you developed in Chapter 2, to include
feedback to the participants. In particular for this task it might be useful to
help participants realize if, for example, they were responding to the color
word rather than the color of the text. You might want to construct your
ultimate study to have a practice period for participants that includes
feedback (to help them get the idea of the task) but then a `main trials`
period where they don't get feedback (such that trials are faster).

Implementation notes
------------------------

You can see that this has been implemented using an additional Routine called
`feedback`. That isn't technically necessary but it is a very easy way to
ensure that feedback always follows the stimulus presentation irrespective of
how long the stimulus/trial lasts (participants have as long as they like to
respond).

The Code Component must come above the Text Component in the Routine, as this
determines the order in which they are executed. If the Code Component comes
lower then the value of `msg` will be updated AFTER the Text Component has been
and the result of this is that it will alter the feedback of the NEXT trial.
Suffice to say that it would be confusing for participants to be given feedback
with a 1-trial delay!

You can copy and paste this Routine to other experiments but you might need to
change the name of the keyboard object to whatever it was called in your study
(in this experiment it was called `resp`). Otherwise you'll get an error that
"resp is not defined".

References
------------------------

Stroop, John Ridley (1935). "Studies of interference in serial verbal reactions". Journal of Experimental Psychology. 18 (6): 643–662.
