Single Page Docs
================

:Authors: Brandon Philips
:Time:
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#brandon-philips
:Link: @BrandonPhilips

Philips is a software engineer who nearly minored in English. At his
previous job he was using technologies that had great docs, and his
company -- although they were creating a great product -- were
creating very poor documents.

So what are some anti-patterns? For example, AWS docs that have a few
sentences or a table, and then click the next link to get the next
paragraph. Or navigate a deep tree that takes lots of navigation.

Single page documents have persistent navigation, utilize scrolling,
and sort of automatically orient you in the document. Scrolling is
natural, like flipping the page in a book in real life. And in single
page documents, search is "free" via the browser. For the
documentation writer, a single page document forces you to think about
the beginning, middle, and end. What's the arc through the
documentation?

A lot of single page documents have persistent navigation that stays
in place as you scroll, so you can easily "thumb" to the table of
contents or to another section. For the author, you're constantly
reminded of how large your sections are getting, and how long the
section names are. Shortening them can really simplify the
understanding of your table of contents.

So terminology is important, and "single page docs" doesn't really
roll off the tongue. The answer: Fixie Docs.

If you're thinking about building Fixie Docs, it's important to know
the downsides. Linking may not be as easy [although it is with Sphinx
:)], users landing from search engines may need to search within the
page again, and your toolchain may not support it easily. Make sure
Fixie Docs are the right match for what you're writing: FAQs probably
aren't the best type of docs for a Fixie.

You can also think about how you split the docs up if you want to go
with multiple Fixies. You wouldn't want to mix tutorials with guides,
for example.

So what tools do you use? Philips started working on a tool for this,
prototype at http://github.com/philips/fixiedocs.
