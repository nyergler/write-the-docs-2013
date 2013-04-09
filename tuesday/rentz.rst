The technical challenges of serving docs at Google’s scale
==========================================================

:Authors: Ashleigh Rentz
:Time: 14:40
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#ashleigh-rentz
:Link:

Ashleigh's business card reads "De-chaos-ifier". She started working
in the data centers at Google as they were starting to grow rapidly.
She started teaching Linux to new hires, and then doing education more
broadly. In 2010, she got involved with technical writers at Google,
and started working on this full time. In 2011 they realized they were
in "big trouble" with respect to developer documentation: there were
so many products that a colleague filled a periodic table with them.
The problems of scale crept up on them slowly, and they didn't realize
how bad it was until it was almost too late.

In 2005 Google hired Chris DiBona from Slashdot and put him in charge
of open source at Google. Part of his job was to help Google
participate in the open source community. They found a few projects
they wanted to release, and put them up on the Codesite,
code.google.com. There were also non-open source projects that needed
API documentation, and the Codesite seemed like the natural place to
put them. Codesite was built using EZT -- Easy Templating -- developed
by Greg Stein, who was working at Google at the time. Just a year
before Google had launched Gmail, and they were churning through
resources. A mandate came down that engineers had to use resources
more efficiently. So Codesite did things like cache things in memory
very aggressively, and was optimized for lots of small files

In 2006 Google launched Project Hosting, and the open source projects
started moving their code or sample code over project hosting. The
wikis were great for the open source projects, but didn't really work
for the API documentation being churned out by technical writers. That
meant that the Codesite started to be solely used for API
documentation, which had different assumptions and requirements.

In 2010 the hourly build was taking longer and longer, and throwing
errors more frequently. EZT was/is unforgiving, and that meant that
the builds wouldn't try to divine your meaning if there was an issue,
it would fail hard. And the build was taking almost the entire hour
between runs. This is in contrast to 2005, when a build and deploy
took 10 or 15 minutes. Consider if something happened, and you
accidentally pushed content that wasn't supposed to be public. It'd
take almost two hours to handle taking that down!

The other thing that changed over time was the desire to start
including code samples. There were lots of XSS vulnerabilities that
got reported.

As Google I/O 2011 was approaching, "Hope" was the strategy they used
as they were shipping docs for new products. And it mostly worked. But
it was stressful, and time consuming. They knew they didn't want to do
the same thing in 2012, so they had to decide between putting a
bandaid on the situation, or hit the reset button and build a new CMS.

They decided to begin work on a new property, developers.google.com,
or Devsite. They had some tools that weren't available for Codesite,
so they built Devsite in Django and django-nonrel on top of Google App
Engine. XSS is dealt with by using a custom template tag that extracts
the demo of the content, puts it into a separate file, and uploads
that to another, non ``google.com`` domain, so it's effectively
sand-boxed.
