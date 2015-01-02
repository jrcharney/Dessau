Dessau
======

No-Frills From-Scratch Software Building for people who just want to make software with what they have available.

## What's in a name?
Dessau is the city in Germany where the famous Bauhaus school of architectural design between 1925 and 1932.  It originally was established in Weimar in 1919, but the city of Weimar until political medelling forced them to relocate in 1925 and ultimately close in 1933 after a short relocation to Berlin when the you-know-whos were taking over.

I had considered calling this project Bauhaus, but there's already a [software project](http://www.bauhaus-stuttgart.de/bauhaus/index-english.html) with that name. Thus I had to think of a different name. (Naming things is hard! I sat here for nearly two hours finding something inspirational!)

The core of Bauhaus design was "form follows function".  The functionism in architecture durning the Modernist Art Period was based on the idea that if you were going to build something, make it functional.  It's form would be secondary to its functionality.  Thus, many buildings build during the Moderinist Era have a very plain look but despite its bland appearance they serve some sort of functionality.

## What is Dessau?

The more I searched for a solution to build things from source, the more I ran into people using other tools like Clang, Linario, and other softwares that don't come with you standard Linux or BSD package unless you cross compile them.  It bugs the hell out of me that I have to install a different C/C++ software compiler because using GCC isn't good enough for some folks.  They want their speed.  I just want to make the damn software!

Thus I've become interested in developing a way to just make software from what's available.  Just as DRY (Don't Repeat Yourself) and KISS (Keep It Simple Stupid) have become good adages in software design, so should FFF (Form Follows Function).

With FFF, we can remind ourself that it shouldn't matter how software is made or what makes it or what it is even made of, just that when is made it should do what we wanted it to do when we thought about it.  It's like writing an essay and staying on topic with an outline as guildance to expresss the main idea.

The idea should come across as clear as possible.  If someone else thinks they can do better, they can fork it.

## What does Dessau do?

Dessau is a set of buildscripts that when run should install software in its most functional form.  If there are some customizations that are necessary, the person building the software need only to look at a list of items available, sort of like `ccmake` only used more.

It will encourage use of GCC, make, Cmake, Python, Perl, and other general software requirements as opposed to going overboard and suggesting to install some other compiler.  DRY, KISS, and FFF aren't just adages, they are laws like gravity.  You won't be punished for breaking the laws, but if you do break them, you'll wish you hadn't unless you can find a very good reason to prove that the laws can be bent or broken.

One of the scripts DEssau will include is a script that installs the Chromium Browser on ARM devices that run Linux.

Dessau scripts will help with the creation of Rigel, Kang, and Kodos by constructing the tools without toiling with third party stuff unless it is easily installed as well.

Basically, if it takes more than a `curl | tar` combo or a `git clone` command to get the software, your working too hard to construct it.  Even more so if the next step after going to the folder the software is in isn't `./configure && make && sudo make install && sudo ldconfig` or `mkdir build; cd build; cmake .. && make && sudo make install && sudo ldconfig`.  However it's made, it shouldn't be rocket science unless you get the software from NASA for making a rocket!
