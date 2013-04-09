Why Projects Should Have “What’s New” Documents
===============================================

:Authors: Andrew Kuchling
:Time: 17:30
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#andrew-kuchling
:Link: http://speakerdeck.com/akuchling/whats-new

Most projects should seriously consider having "What's New" documents
as part of their standard documentation set. Kuchling wrote the
*What's New* documents for the Python 2.x series of releases. This was
largely his contribution to python-core for the better part of a
decade.

The goal with What's New documentation is filling in the gaps. The
README may say "Introduced generators and iterators", but that's a lot
of changes described in a single sentence. There's also the NEWS file
(changelog), but that's a level of detail that doesn't really tell
users if each change is going to impact their code.

So the user benefits are clear, but there are benefits for the
developers, as well. Obviously "What's New" docs help fill in the gaps
between README and NEWS, but they're particularly useful for users who
have upgraded their Python distribution. The tutorial style also makes
it approachable for new users.

For developers, What's New makes it easy to answer the historical
question of "when was this feature implemented or added to the
project?" It also helps provide a guidebook for the alternate
implementations of Python (Jython, Iron Python, etc).

When writing What's New documents, Kuchling created a skeleton
document when each development branch was created. Over time he
developed an ordering: meta changes (bug trackers, source control,
etc), PEPs (numerically ordered), and then changes. He subscribed to
python-checkins, and periodically spent an evening processing them.

The editorial policies were:

* Be useful to the reader.

  The imagined user was an intermediate Python user who didn't follow
  ``python-dev``. This often meant creating mini tutorials for new
  features, and providing background material when necessary (for
  example, when Decimal was added to the language). He also tried to
  provide pointers into Python's development process when useful:
  links to bugs in the tracker, mailing list threads, etc.

* Focus on changes of wide interest
* Write new explanations and examples instead of writing new PEPs or
  docs.

  The rational is that this provides yet another explanation, which
  could help people understand a new feature.

Writing What's New documentation takes time, but it's worth it to
provide more comprehensive support for users.
