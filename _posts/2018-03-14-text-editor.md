---
title: "Updating my text editor"
tags: [programming, opinion, misc]
---

The text editor is likely the software in which programmers (and those who sell themselves like ones, i.e. myself) spend the most time,
thus it is vital that the tool of choice is up to the job. However, choice of the code editor is [somewhat controversial](https://xkcd.com/378/).

In the core software engineering classes we had religious battles over which one should use;
some preferred vim, some swore by [Atom](https://atom.io/), and some were using [RStudio](https://www.rstudio.com/), because "C is not _that_ different from R, and it has latex support".

As ever, I had a strong opinion on the matter as well.

Vim and emacs made my programming less efficient than it should have been. They are
great tools, and can work wonders, but the steep learning curve and some features of "more modern" text editors
made me avoid them on my personal computers (although I do use vim on the workstations without the GUI and it is quite awesome).

On the other hand, editors like Atom made me feel like I was using a browser - good for watching porn, and wasting time,
but not too efficient for anything else. I've tried Atom in its early days and was severely disappointed.
It would freeze when opening large projects, crash while updating, and cause more problems
then it solved, and I'd experience input lag on even the smallest projects such as editing this blog.
The larger projects such as torch would seldom even start up.

[Sublime](https://www.sublimetext.com/) was a nice middle ground - it was lightning fast due to the native C++ implementation, and it had a plethora of plugins (provided you
installed package control) and code editing features that made my life easy enough, and since they were implemented in python easily modifiable as well.
The only real problem with Sublime was the initial setup time to get things where I want them. And the fact that you had to do it on every new computer,
and it never ended up feeling quite the same. There have been workarounds for such issues such as [unofficial Dropbox sync](https://packagecontrol.io/docs/syncing), but I found that would reload my editor every time my dropbox synced (which itself was handled in a very weird fashion on Linux). And if I wanted to use it on the computer where I
didn't have my personal dropbox synced (i.e. department provided workstation), ... I guess I could script things?
One other silly thing is that it was a closed source - paid for application. For some reason, I grew more and more fond of the idea of having my basic
setup open-sourced and platform independent, and if possible, free.

Last summer, while working at MS, I needed something with simple text capabilities. Visual Studio/ReSharper combo was great for working with C#, but doing basic
text editing was still easier to do in a text editor. Setting up sublime seemed like a major pain, because a) my license was paid for by another company, and b) it would
take a while to set it up to work with my new environment (i.e. not developing python/lua anymore). Notepad++ was annoying as I used a Linux VM and it wouldn't be
transferable. I decided to support the local guys and installed VS Code not expecting much.
It worked really well out of the box and had the support for everything that I needed, including an automatic switch to sublime key bindings. It was a bit slower
on startup than sublime, but it didn't feel like a porn watching tool, which is a big plus. I've pushed "dabble with VS Code" on my stack and forgot about it for a while.

Two weeks ago, while waiting for a couple of TB of videos to download, I figured, it's as good of a time as ever to "dabble with VS Code". Again, setup was straightforward enough
on both my Linux workstation and Apple laptop. I installed the recommended plugins for the type of work that I am doing, and decided to try it exclusively until the end of the
month, and see whether it is worth switching to. Here is the initial opinion:

# Setup

I've been using the latest setup extensively for the last 20ish days for the following tasks:

1. pytorch development: minor contributions and bugfixes to the pytorch repo
2. maintenance of some legacy Lua code (torch relics)
3. work on my own pytorch and caffe2 projects
4. this blog
5. editing .tex documents

I've used it on the latest macOS, Ubuntu 17.10 and latest Fedora. To find the complete list of plugins, look at the bottom of the post.

## The good

- __support__: any questions and weird issues that I have while messing up with plugins were responded to by either the VS Code twitter guys or dedicated plugin developers in less than an hour. For some reasons every forum and group dedicated to VS Code seems to be exceptionally active. [People clearly love it](https://insights.stackoverflow.com/survey/2018#technology-most-popular-development-environments), and it's becoming easy to see why.
- plugins: the fact that it's effectively a browser does make it infinitely extensible, and I love the built-in terminal, python linting and intellisense that ties with the env you are it is an awesome feature. I can jump between my caffe2 and pytorch projects, and have my code analysed accordingly.
- design: it looks nice, and it's well thought through; fonts are rendered with no issues on every OS
- __sync__: with the sync plugin, everything is in a gist, and can be synced by simply generating the new access key. No fuss, no problems, takes 30ish seconds
- out of the box configuration: everything built in works, and it works remarkably well.
- __git diff view__: I've never had an issue with command line git workflow, but this feature (that I first saw in the full version of VS) makes it that much more convenient
- geekery: I love the fact that devs take the time to geek out about improvements they made in [changelogs](https://code.visualstudio.com/updates/v1_21). I learned about new data structures and the inside-outs of it through their changelogs

## The bad

- __startup speed__: it takes a few seconds post starting for everything to load. Thankfully, that's where the similarities with porn sites end
- updates: when it updates, it is still a bit of a mess. However, it never crashed and burned as Atom did some years ago.
- typescript: if I want to modify a plugin in Sublime, it's a breeze. Not knowing typescript is a disadvantage here.
- workspaces: not sure if they work as well as Sublime's projects do. This one will take time to validate properly

# Verdict

It's too early to say, but I think this one is a keeper.
I learned to love it and started to lean towards it as my main editor. It doesn't mean that I'll get rid of sublime, however
**VS code just became my go-to editor**. It really is that good.

---

List of plugins at the time of writing:

- Anaconda extension pack
- Git Project manager
- markdownlint
- Material Icon Theme
- One Dark Pro Theme
- prototxt
- Python
- Settings Sync
- sftp
- Spell Right
- Todo+
- VS Code Jupyter Notebook
- YAML Support by Red Hat
- Git Lens
- Git History