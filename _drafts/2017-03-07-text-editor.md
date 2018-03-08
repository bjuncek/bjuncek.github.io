---
title: "Updating my text editor"
tags: [programming, opinion, misc]
---

Text editor is likely the software in which programmers spend the most time,
thus it is vital that the tool of choice is up to the job.

In the core software engineering classes we had religious battles over which one should use;
some preferred vim, some swore by atom, and some were using RStudio, because "C is not _that_ different from R".

As ever, I had a strong opinion on the matter as well.

Vim and emacs made my programming less efficient than it should have been. They are
great tools, and can work wonders, but the steep learning curve and some features of "more modern" text editors
made me avoid them on my personal computers (although I do use vim on the workstations without the GUI and it is quite awesome).

On the other hand, editors like Atom made me feel like I was using a browser - good for watching porn, and wasting time,
but not too efficient for anything else. I've tried atom in it's early days and was severely disappointed.
It would freeze when opening large projects, crash while updating, and cause more problems
than it solved, and I'd experience input lag on even the smallest projects such as editing this blog.
The larger projects such as torch would seldom even start up.

Sublime was a nice middle ground - it was lightning fast due to being a native C++ implementation, and it had a plethora of plugins (provided you
installed package control) and code editing features that made my life easy enough, and since they were implemented in python easily modifiable as well. 
The only real problem with Sublime was the initial setup time to get things where I want them. And the fact that you had to do it on every new computer,
and it never ended up feeling quite the same. There have been workarounds for such issues such as unofficial Dropbox sync, but I found that would reload
my editor every time my dropbox synced (which itself was handled in a very weird fashion on Linux).
One other silly thing is that it was a closed source - paid for application. For some reason, I grew more and more fond of the idea of having my basic
setup open-sourced and platform independent, and if possible, free.

However, last summer, while working at MS, I needed something with simple text capabilities. Visual Studio/ReSharper combo was great for working with C#, but doing basic
text editing was still easier to do in text editor. Setting up sublime seemed like a major pain, because a) my license was paid for by another company, and b) it would
take a while to set it up to work with my new environment (i.e. not developing python/lua anymore), and Notepad++ was annoying as I used a Linux VMs and it wouldn't be 
transferable. I decided to support the local guys, and installed VS Code not expecting much.
It worked really well out of the box, and had the support for everything that I needed, including an automatic switch to sublime key bindings. It was a bit slower than
sublime, but it didn't feel like a porn watching tool, which is a big plus. I've pushed "dabble with VS Code" on my stack and forgot about it for a while.