Stroop with current trials progress
=============================================================

In many experiments you want to provide information about how far through the
trials/survey the participant has got. Here is a simple demo of how to make
that work.

Solution
------------------------

We've actually gone a bit further than the exercise/solution in the book as
well, because we've added this feature to the solution from Exercise 6.1,
which had a practice loop as well as a trials loop, and which already had a
`msg` being defined for feedback. As a result we have changed the solution
slightly from what the book described:

  - we've now called our message variable `progressMsg` so that it won't clash
    with the `msg` variable being used to provide feedback
  - referring to `trials.thisN` and `trials.totalN` in this version would not
    have worked in the `practice` loop. It would have resulted in an error
    that "trials has not been defined" at that point. So, instead, we have
    used `currentLoop.thisN`, `currentLoop.nTotal` which will works the same
    but applies to whatever loop is currently running rather than a specific
    one.

References
------------------------

Stroop, John Ridley (1935). "Studies of interference in serial verbal reactions". Journal of Experimental Psychology. 18 (6): 643–662.
MacLeod, CM (1991). "Half a century of research on the Stroop effect: an integrative review". Psychological Bulletin. 109 (2): 163–203.
Peirce, J.W. and MacAskill, M. (2018). "Building experiments in PsychoPy." Sage Publishing.
