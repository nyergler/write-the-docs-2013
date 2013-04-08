Motivating developers to write API documentation
================================================

:Authors: Jennifer Hodgdon
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#jennifer-hodgdon
:Link:

Let's dispense with the question of whether or not you *need* API
documentation. You do. But how do you get it written? There are sort
of three options: no one writes docs (not desirable), hire technical
writers (which works one corporate projects, but there's potential for
drift knowledge between the developers and the writers), and finally
having the developers write the docs themselves. The latter option is
probably the only viable solution for open source projects, and may be
desirable in a corporate setting, as well.

When Drupal 7 shipped, there was a lot of improvement to the API
documentation, primarily because jhodgdon (the speaker) was very
motivated. She contributed 278 patches, and was #6 in terms of overall
number of patches. But this isn't sustainable, and it doesn't scale.
So when the Drupal 8 cycle began, there was a decision to enlist the
entire community to help. In addition to the written standards for
code, there were standards created for docs
(http://drupal.org/coding-stnadards/docs). There were also cultural
changes: bad documentation is considered a bug, and patches without
minimal documentation are unacceptable.

Drupal 8's cycle introduced the idea of "core gates". When the
community reached the end of the Drupal 7 cycle there was lots left to
do for usability, documentation, test coverage, etc. Drupal 8
introduced the idea of gates that patches have clear
(http://drupal.org/core-gates). These aren't enforced perfectly, but
there are common goals that everyone is aware of.

The Documentation Gate says that all functions, classes, etc have to
have at least minimal API documentation blocks: one line summary,
documented parameters, return values documented. Clarity is required,
grammar is optional on the first pass. They also consider code
comments as internal documentation. Finally, there should be
documentation for API changes.

So how did they get it done? Well the API documentation is embedded
with the source, so you can fix it with the standard code patch
process. There's a "report a bug" link on their API site, which lets
people notify the developers of issues. Easy documentation bugs
reported this way are tagged as "novice", and they've found that bugs
marked this way are fixed within a week. Novice bugs (and the people
that fix them) are supported by the "Core Office Hours" mentoring
program (http://drupal.org/core-mentoring). Finally, there's a
dedicated API docs patch reviewer/committer.
