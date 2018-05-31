Stroop with practice that detects high performance
=============================================================

Often a set of practice trials can be aborted once participants have reached
some criterion performance on it, which is the aim of this exercise.

This exercise extends the second extension we made to the Stroop task, in which
we added a practice loop and provided feedback on the average performance over
the last 5 trials (Chapter 6).

Here we will use that same code to measure the number of correct responses in
the last 5 trials, but then we'll also abort the loop if the participant gets
to a threshold level of (say) 4 out of 5 correct responses.

Implementation
----------------

Take a look at the code that has been added to the `feedback` Routine, in the Code
Component called `message`.

References
------------------------

Stroop, John Ridley (1935). "Studies of interference in serial verbal reactions". Journal of Experimental Psychology. 18 (6): 643–662.
MacLeod, CM (1991). "Half a century of research on the Stroop effect: an integrative review". Psychological Bulletin. 109 (2): 163–203.
