# Day 2: 1 July 2025 - Cambridge Digital Humanities

## Digital Humanities at the Command Line

The practical sessions today will focus on the command line. This is one of the 'glue' skills for RSE work but is often picked up piecemeal, and not just by DH people: MIT have a [missing semester](https://missing.csail.mit.edu/) for Computer Science degrees, where the command line (or shell), features prominently.

One of the benefits of command line knowledge it that much of it is transferable. If you find yourself on a machine, or even a server, where the software you're used to (Python, for example, or your favourite text editor) isn't available, there is a very good chance that what we cover today will be.

**Lead**: [Jonathan Blaney](https://www.cdh.cam.ac.uk/about/people/jonathan-blaney/)

## Pre-Workshop Preparation

### Installation and accounts

You will need three things for the day: a laptop, a Unix terminal program and a Google account. The Google account allows you to use Colab for the Python session at the end of the day.

If you have a Mac or Linux laptop then you don't need to install anything. If using a Mac, you may optionally install [iTerm2](https://iterm2.com/), which is a bit more user-friendly than the built-in Terminal program, and is what we will use to demonstrate. However this is mostly cosmetic and Terminal will meet your needs perfectly well.

We will expect Windows users to have the free Git Bash program installed. If you have Windows Subsystem for Linux enabled, you should already have it. If not, you can install it as part of [Git for Windows](https://gitforwindows.org/). Please check that it is working before the day. We will **not** be using or supporting PowerShell or DOS, the command line programs that come with Windows 11, because the commands differ substantially.

### Downloads

We will use some files for practice and then for the challenge session and we recommend downloading them in advance. From [Project Gutenberg](https://www.gutenberg.org/) we will be using their unwieldy plain text list of books and ebooks linked to as `GUTINDEX.ALL` on [this page](https://www.gutenberg.org/ebooks/offline_catalogs.html). Please also download a modified version of this file, `gutenberg.tsv`, where the key information is all on one line (you will find the file in the [`Day 2`](https://github.com/kingsdigitallab/dh-rse-summer-school-2025/tree/main/Day%202) directory listing, at the top of the page).  

For the challenge we will be using the text of Milton's _Paradise Lost_. The text also comes from Project Gutenberg, but we recommend using a slightly cleaned up version, `paradise-lost.txt` (also in the [`Day 2`](https://github.com/kingsdigitallab/dh-rse-summer-school-2025/tree/main/Day%202) directory listing).

### Preparation

We won't assume any prior knowledge of the command line, but many attendees have indicated that they have some experience. We will introduce fundamentals such as navigation and file operations, but only briefly. If you're new to to the command line, you will have a better experience on the day if you've already practised a bit (but don't worry about understanding everything you come across).

There are many online tutorials. This [Introduction to the Bash Command Line](https://programminghistorian.org/en/lessons/intro-to-bash) from the excellent [Programming Historian](https://programminghistorian.org/) site covers the basics well and without assuming any previous knowledge (but note that things like installation instructions may be out of date).

We will cover these movement commands: [`cd`](https://en.wikipedia.org/wiki/Cd_(command)), [`ls`](https://en.wikipedia.org/wiki/Ls), [`pwd`](https://en.wikipedia.org/wiki/Pwd).

And these file commands: [`cp`](https://en.wikipedia.org/wiki/Cp_(Unix)), [`mkdir`](https://en.wikipedia.org/wiki/Mkdir), [`mv`](https://en.wikipedia.org/wiki/Mv_(Unix)), [`rm`](https://en.wikipedia.org/wiki/Rm_(Unix)).

We will also introduce commands that you might want to use in the group exercise: [`cut`](https://en.wikipedia.org/wiki/Cut_(Unix)), [`grep`](https://en.wikipedia.org/wiki/Grep), [`sed`](https://en.wikipedia.org/wiki/Sed), [`sort`](https://en.wikipedia.org/wiki/Sort_(Unix)), [`uniq`](https://en.wikipedia.org/wiki/Uniq), although the choice of commands will be yours.

Beyond the Wikipedia pages linked above, you can use the `man` pages from the command line, like this:

`man cp`

Press `q` to exit.

However Git Bash does not come with a built-in manual so you may want to consult the [online version](https://www.man7.org/linux/man-pages/index.html) instead.

If you want to go further, there is a useful [table of commands](https://en.wikipedia.org/wiki/List_of_POSIX_commands) on Wikipedia, and [Daniel J. Barrett's](https://danieljbarrett.com/books/) _Linux Pocket Guide_ and _Efficient Linux at the Command Line_ are full of good information and not very Linux specific. 

## Schedule

- 09:00-09:10 Mini-talk: Society of Research Software Engineering (Mary Chester-Kadwell)
- 09.10-10:30 Humanities RSE work at Cambridge (Estara Arrant and Mike Hawkins)
- 10:30-11:00 BREAK
- 11:00-12:30 The command line: principles and best practice (Jonathan and Ryan)
- 12:30-13:30 LUNCH
- 13:30-15:00 Command line group challenge: Building a complex pipeline (group work)
- 15:00-15:30 BREAK
- 15:30-17:00 Distant reading with the command line and Python (Ryan and Jonathan)

## Speakers and Trainers

- [Ryan Heuser](https://www.cdh.cam.ac.uk/about/people/dr-ryan-heuser/), Cambridge Digital Humanities
- [Estara Arrant](https://www.lib.cam.ac.uk/collections/departments/taylor-schechter-genizah-research-unit/unit-staff/dr-estara-arrant), Leverhulme Early Career Research Fellow, University of Cambridge
- [Mike Hawkins](https://www.cdh.cam.ac.uk/about/people/dr-michael-hawkins/), Senior Developer, Cambridge University Library

## Abstracts

### Estara's talk

I will be speaking on the challenges, high points, and experiences of navigating a data science/research software engineering career in the Humanities from a solo researcher perspective. I will also discuss the challenges of  effectively communicating and collaborating in such a cross-disciplinary environment. In particular, I will cover include my entry into this area, how I am maintaining and further developing my skills, and the future paths are  potentially available. I will touch upon ways in which I think people can effectively enter and navigate this field, with a view to its developments."

### Mike's talk

'An Accidental Digital Humanist'

There are many different pathways into a career in the Digital Humanities. This is not surprising considering that the ‘digital humanities’ in most universities has a long and varied history that predates the establishment of official centres and degree programmes. The University of Cambridge is no exception. This helps to explain how a historian of early modern science ended up working for over twenty years on a wide range of digital projects. In my talk, I’ll discuss my activities on some of the key projects I’ve worked on at Cambridge, such as the [Casebooks Project](https://casebooks.lib.cam.ac.uk/), the [Darwin Correspondence Project](https://www.darwinproject.ac.uk/), and [Unlocking Digital Texts](https://textframe.io/), as well as my current duties as a Senior Developer at the Cambridge University Library.



## On-the-day Slides and Instructions

These will be added shortly
