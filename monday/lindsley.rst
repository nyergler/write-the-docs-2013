The Unenviable Tutorial
=======================

:Authors: Daniel Lindsley
:Time: 16:40
:Session: http://docs.writethedocs.org/en/2013/conference/talks.html#daniel-lindsley
:Link: @daniellindsley / http://github.com/toastdriven

Lindsley is the author of several decently-used Python/Django
libraries, which pride themselves on having good (maybe not great, but
good) documentation. Lindsley prides himself on having good docs,
because good docs are the difference between evaluation and adoption
of software.

So what makes the tutorial "unenviable"? It has the single worst job
of any piece of documentation in your project.

* It's the first doc people see.
* It's often one of the first documents written.
* That means it's often one of the first pieces of documentation to
  fall out of date. As the developer, you don't *need* the tutorial.
  You don't use it, so it's more prone to rot.
* The tutorial must pull users in to be effective.
* The tutorial sets the standard for how your library should be used.
* It needs to describe *just enough*... if you tell them too much, new
  users will feel overwhelmed.

The tutorial is unenviable because it's expected to be everything to
everyone. So how do we make it better?

First, what not to do.

* RAD (READMEs as Docs) is not rad: your README is not a doc, it's
  organizational. READMEs need to pull together a lot of different
  pieces of information, so they're not appropriate for new users.
* Showing off every single feature overwhelms new users, and probably
  isn't the best format for advanced users.
* Immediately deep diving into specialty portions of the technology.
* Writing solely for the advanced user: they're not the target
  audience for tutorials.

Considerations for the Tutorial.

* *Both* the novice and pro users will land there coming from Google.
* The tutorial needs to prove the software's worth.
* A good tutorial should be "lunch hour"-able: something a new user
  can go through during the lunch hour and receive an introduction to
  the software.

So how do you construct the tutorial generally?

#. Have empathy for your users: Where are your users coming from?
   What's the problem that they have?
#. Pick the easiest-to-bite-off features first.
#. Start simple. What's the smallest chunk that will get something
   working fast?
#. Use small iterations: build on what you've already taught.
#. Speak clearly and simply with friendly prose. Expand on
   new/difficult concepts, and engage the user with your text.
#. Write for the new user, but [paradoxically] make it easy for the
   advanced user to skim and absorb.
#. Know when to stop: the tutorial shouldn't exhaust a user, delve
   into the depths of the API, or try to cover everything. Don't
   overwhelm your reader.

Common pitfalls

#. Making assumptions about what the reader knows.
#. Diving too deep, too quickly.
#. Or unfortunately not showing enough. Going too shallow makes it
   look like your project isn't going to meet the reader's need.
#. All examples, no prose: you need narrative connectivity in your
   tutorial.
#. Don't leave the user hanging at the end: where does the user go
   next? What's the logical next step? Does the user have choices?

So now what? Now it's time to write the *guides*. Topical guides are
like tutorials, but focused on a particular topic. How do you enable
specific behavior? How do you adapt to certain situations? Guides are
a good way to help users dig in. Your guides and the tutorials should
be inter-linked. There's no excuse on the web: use links! Once you
have some documentation, run it past friends and co-workers. Even
smart lay people can give you important feedback. Finally, let users
know where they can go for help when they need it (IRC? mailing list?
forum?).
