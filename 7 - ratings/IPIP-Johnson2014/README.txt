IPIP-NEO-120 Personality measure
============================================================

The instrument
------------------------

This is a simple implementation of the IPIP-NEO-120 personality scale, a fairly
brief (120-item) measure of personality across 5 factors and and 6 "facets"
within each of the 5 broader factors. This was based on the larger (300-item)
IPIP-NEO by Goldberg (1999) which, in turn, aimed to measure the same factors
as the commercial tool by Costa and McCrae (1992). Both the IPIP-NEO-120 and
IPIP-NEO are freely available as public domain resources at http://ipip.ori.org

Note that this demo is provided as an educational tool, teaching you how to use
rating scales in PsychoPy, rather than as a clinical tool. Working with
psychological tests takes a great deal of experience and training that is
beyond the scope of this text.

Implementation notes
------------------------

This PsychoPy version of the test allows a 5-point Likert scale as in the
original but differs a little in that only one item is ever presented at a time
and participants cannot return to a previous item. In Johnson's web-based
implementation the items are all presented on a single page and participants
are able to alter the answers afterwards and in any order.

References
------------------------

Johnson, J.A. (2014). Measuring thirty facets of the Five Factor Model with a
  120-item public domain inventory: Development of the IPIP-NEO-120.
  Journal of Research in Personality, 51:78–89

Goldberg, L. R. (1999). A broad-bandwidth, public domain, personality inventory
  measuring the lower-level facets of several five-factor models.
  In I. Mervielde, I. Deary, F. De Fruyt, & F. Ostendorf (Eds.).
  Personality Psychology in Europe (Vol. 7, pp. 7–28).
  Tilburg, The Netherlands: Tilburg University Press.

Costa, P. T., Jr., & McCrae, R. R. (1992). Revised NEO personality inventory
  (NEO PI-R and NEO five-factor inventory (NEO-FFI): Professional manual.
  Odessa, FL: Psychological Assessment Resources.
