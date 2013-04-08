Typography for Docs
===================

:Authors: Matthew Butterick
:Time: 11:00
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#matthew-butterick
:Link: http://www.typographyforlawyers.com/

Before computers the most amazing machines were type foundries and
presses. So programming and typography have a lot in common. In 1994
Butterick went to a type design conference in San Francisco where he
ran into some friends. They were programming with a "great new
language" invented by one of their brothers: Python. In 1994 he wasn't
working in Python, he was working in C, because he was writing
software to do better kerning on a Mac. The K&R C book [he holds up]
holds reader attention, partially because it's an accessible size,
it's approachable, and it's functional.

Typography can be decorative, but it serves a functional purpose: it's
supposed to hold (and conserve) reader attention. Once the reader --
of your book, of your documentation -- checks out, it doesn't matter
how good the content is (or could be). Holds up an AppleScript book --
"NINE HUNDRED PAGES! WHAT IS THERE TO SAY ABOUT APPLESCRIPT THAT TAKES
900 PAGES!?!" [Shows a picture of OReilly's Programming Python] "WHAT
HAPPENED, PYTHON!? WHEN DID YOU GET SO FAT?" This is not what
programming Python is about! Even "Learning Python" is 800 pages long,
and what is there to say? It's *interesting* that K&R is so slim, since
when Butterick was reading it in 1994 there wasn't Google, there
wasn't Stack Overflow, and today you have all these backup sources of
documentation to draw from.

[Refers to a picture of the butterfly ballot from Palm Beach, FL in
2000.] "This piece of jack-ass typography got us into WAR!" The
problem is a matter of reader attention: the ballot sort of makes
sense if you have twenty minutes to look at it, but voters don't
necessarily have that long in the voting booth. The ballot didn't
*conserve* reader attention.

So Butterick isn't attempting to teach us to be typographers (those
who design with type), because we're already that if we're putting
words onto a surface. There's talk on "no design" or "anti design",
which doesn't make a lot of sense, since how do you put words on a
page *without* designing it? (Poorly or well is another question.)

So many college professors hold on to conventions from the days of
type writers: 1 inch margins, 12 point type, Times New Roman. Why do
we hold onto those things? And if you say "I'm only on the web, man",
well in some ways we're still re-enacting the early typography
problems of the early web.

The body text determines how appealing or awful your document is. It
*has* the greatest influence, because it's the most prevalent. There
are four factors that affect how the body text looks.

#. Font choice. A lot of people thing Verdana and Georgia are the
   "great" web fonts. Yes, in 1996. But things were different: screens
   were smaller and anti-aliasing sucked. They're still fine, but they
   were designed for a particular time and place. There are some great
   open source fonts: Charice (? not sure I got this right), Charter_
   (now open sourced by BitStream), and `Source Sans`_. (Rant on
   Google open source fonts: they don't really reflect an open source
   ethos, because they're the work of an individual and not
   collaboration. There weren't a lot of eyes to make the bugs
   shallow.)

   Arial and Verdana don't represent a choice, they represent a lack
   of choice. Just like the black nothingness of space isn't a color,
   so much as the absence of all light.

#. Font size. Twelve Point is a hold-over from typewriters. If you
   look at most printed work, it's set at 9pt to 11pt, because paper
   costs money! In the early days of the web, the easiest way to make
   the anti-aliasing look better was to *make it bigger*.

#. Line length. In addition to font selection, this is the thing
   almost everyone gets wrong in typography, and it's easy to get
   right. The problem with really wide lines is that they're really
   uncomfortable to read. Why they're uncomfortable doesn't really
   matter, we're used to reading something like 45 to 90 characters.
   [YES! PEP-8!] This is the Plank constant of line length. An easy
   way to remember this is that it's two to three lowercase alphabets.

   [Shows example of redesigned Bottle front page that shrinks the
   line width, and it *does* look easier to read.]

   If you look at the documentation for Python-Lex-Yacc, you'll see
   that it's way too wide! It's 1995 responsive design with no concern
   for width, which worked then, because the screens were smaller. And
   Sphinx is problematic here, too, because it's doesn't respect the
   rules about line length.

#. Line spacing: the vertical distance between lines. This should be
   120% to 145% of the font point size. Just do it.

Readers are coming to your documentation site to DO SOME READING! The
adornment, the non-text DOESN'T MATTER! Headings don't have to be
HUGE, they just need to be a little bit bigger. And on the web, where
you have essentially unlimited vertical space, white space is a very
effective way to separate content.

Demonstrates making text scale as you resize the browser. Uses @media
queries with max-width, generated by a Python script.

.. _Charter: http://en.wikipedia.org/wiki/Bitstream_Charter
.. _`Source Sans`: http://blogs.adobe.com/typblography/2012/08/source-sans-pro.html
