Literate Programming in the Large
=================================

:Authors: Tim Daly
:Time: 11:00
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#tim-daly
:Link:

"I'm here to tell you you're doing it wrong. I'm also here to tell you
that you're god-like figures and you don't even know it."

Axiom is a computer algebra system that Daly worked on at IBM
Research. It was the first computer algebra system, and handled
solving lots of sorts of equations. When funding was cut by the Reagan
administration, IBM decided to sell the software, which meant that it
needed to be documented. At the same time, there were severe memory
limits, which meant that the programs were often constructed as small
files. When the buyer, NAGS, decided to take it off the market, they
were going to throw it away. Daly asked if he could have it, and they
said yes.

It took Daly about a year to put the code back together, and then he
open sourced it. He realized that he could tell you what segments
would *do*, but couldn't tell you *why* it had to be in there. It was
1.2 million lines of Common Lisp without any comments. There wasn't
any sense of "why", and Daly realized that's what was really missing.
Knuth had previously pointed out that we shouldn't be writing programs
for computers, we should be writing them for human readers.

When we do code reviews, it's often difficult to comment on anything
beyond the cosmetic or glaring: you don't have the context for what
the programmer is trying to do, what their task is. But if you can
provide a page or two that explains what's going on along with the
code, that provides context and background. If you do that enough, you
wind up with a "book" that explains the system.

So Daly has been working on Axiom, and it's still more than a million
lines of Common Lisp. It's also a million lines of literate LaTeX.
