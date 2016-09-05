.. title: Cutting your A0 LaTeX document into multiple A4
.. slug: cutting-your-a0-latex-document-into-multiple-a4
.. date: 2016-09-05 00:38:56 UTC+02:00
.. tags: latex,poster
.. category: 
.. link: 
.. description: 
.. type: text

One of the forms of conference participation is a poster presentation. You're supposed to create an A0 [#]_ document with graphs and brief explanation of your work, hang it in the designated area and show up during the poster session. Other participants would do the same, and the whole session usually lasts a couple of hours. The idea is that eventually you get bored standing next to your poster, and go around asking questions. The other people do the same, and, therefore, you communicate with each other, discussing science.

Making poster with LaTeX
========================

There're basically not that many programs that you can use to create an A0 poster. Especially if you have some of the results in LaTeX and you would like to reuse them, and not a fan of Adobe Illustrator (or InDesign, or Inkscape, or whatever other vector graphics editor). In LaTeX there are, basically, two classes for a poster --- `beamerposter <https://github.com/deselaers/latex-beamerposter>`_ and `tikzposter <https://bitbucket.org/surmann/tikzposter/overview>`_. There are a few other packages [#]_ that allow you to do a big A0 document, but I believe these two are the most popular ones. Beamerposter is related to beamer, the only reasonable LaTeX package to create presentations. It is is most usefull when you have a presentation that you want to turn into poster with as litlle pain as possible. If you don't have a presentation like that, its document structure might feel unnatural. Most of the time I use tikzposter and I'm quite happy with it.

Making poster on time and failing
=================================

Recently, however, I had an unpleasant realization that I won't be able to get my poster printed on time [#]_. So I had to resort to cutting my poster in pieces and bringing the resulting bunch of 16 A4 sheets with me as my poster. In hindsight, I should have realized that our University printers are capable of printing A3 sized documents. I even done that, but I assume I was too stressed that evening. Luckily, I stumbled upon `this stackoverflow post <http://tex.stackexchange.com/questions/171500/how-to-print-a0-poster-as-an-array-of-combinable-a4-pages>`_, that worked flawlessly. Well, almost flawlessly. I managed to screw up and print a wrong poster, and I only noticed it once I got to the hotel where the conference took place :) Again, the stuff at the reception were super friendly and they had an A3 printer, so I solved my problem by reprinting it there. No big deal in the end.

Lesson learned (hopefully)
==========================

A couple of things I learned from this experience:

  * That saying "Score twice before you cut once." [#]_ is extremely applicable when you cutting the poster. And I mean it not only in a sense of being pixel-perfect, but also checking **which poster you're cutting before cutting it**. I accidently printed wrong poster but failed to notice it. I was too excited finding a minimal amount of cuts I need to make a perfectly overlapping picture.
  * If going for A3 paper size, make sure to set ``a3paper`` option for ``\documentclass`` command. Otherwise there might be trouble printing it. Especially, if you're not the one sending it to print (I had exact this problem first time we tried to print it on the hotel reception's printer)
  * Travelling with a few sheets of paper is much easier than traveling with a poster tube. If you know that the conference is somewhere far, it might be a good idea to have a tactically enhanced A4 poster. That is, a series of interconnected A4 pages with huge graphs and big readable fonts.

Anyway, just to make it easier to access, I put the tex files to cut the A0 poster into multiple A4 (or A3) in `my repository of LaTeX templates <https://github.com/cra/One-page-latex-templates>`_. Though I do hope I won't need this particular ''lifehack'' anytime soon.
    

.. [#] Though I had one conference where A1 was the recommended poster size, I think it's quite uncommon.
.. [#] I once heard a story about some guy doing his poster with a0poster, but I'm not sure if that person was sane
.. [#] No one to blame for this but me. I handed my poster to our University's typography way too late before the conference's start.
.. [#] Funny, but the similar proverb stays you need to score 7 times. Didn't help in my case though :D
