How Mozilla Supports Users All Over the World
=============================================

:Authors: Michael Verdi
:Time: 9:40
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#michael-verdi
:Link: http://mzl.la/wtd

Verdi is the content manager on the Sumo project: support.mozilla.org.
Sumo supports Firefox, Firefox for Android, Firefox OS to 450 million
people around the world, on every continent (including Antarctica).
These users speak 80 different languages. There are thirteen paid
staff and three developers working on the support team, up for four
only a few years ago. The project works by (spoilers!) writing a lot
of documentation, putting it on the web, and then localizing it into
all the languages. At any given time there are around 200 people
contributing in some fashion. They have a posse. These are
superheroes, but not like Superman, like Batman: tech, not powers.

They start with proactive support: user advocacy and education. The UA
team advocates for fixing things that they know will be user impacting
they become pain points that *need* to be documented. The also
advocate for things like the "Reset Firefox" button, which makes it
easier to write troubleshooting documentation. The education team
builds up videos and support documentation that gets included in the
marketing pitch to news sites when a new release goes up. That results
in more views, more exposure.

If education and advocacy doesn't work, Mozilla employs reactive
support using `Kitsune <https://github.com/mozilla/kitsune/>`_, their
support software. This includes the knowledge base, a Q&A style
support forum, Twitter client, internal communication, and metrics.
The knowledge base is wiki based and supports localization, multiple
products (and versions), and multiple operating systems. It has
support for templates for frequently repeated tasks, and a review
system for content review.

When it comes to supporting multiple operating systems and Firefox
versions, Kitsune allows them to include the instructions in a single
document, and when the visitor comes to the site they'll see the
sections/content that's appropriate for their operating system and
software version (if applicable).

The review system allows them to review diffs to documentation,
provide feedback to authors, and mark content as ready for
localization. It also supports putting together a document level to do
list.

If you visit a wiki document that hasn't been localized (ie, you're
browsing from France and visit an unlocalized English document), they
show a link above the text that links to the localization
documentation. If you're already logged in, there's a link in the
sidebar to "Translate this Article", that shows a side by side editor.
And because a large majority of the traffic focuses on the top 100
documents, the dashboards can highlight the things that contributors
should work on (the highest traffic). When you're updating a document
that was previously localized, you'll see a red/green diff in the
English text.
