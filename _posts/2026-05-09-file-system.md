---
layout: post
title: "Usage of Seminar"
author: "Tianyi Xie" 
categories: Tools
---

> This article talks about how I organized my files. 

As graduate students sometimes we feel the need to make our file system more organized. WIth increasing number of notes, papers, codes and textbooks; pdfs, mds and more and more Jupyters, they bother me by being hard to find or even lost when my laptop is broken. Then I summarize the needs: 

- Well organized by file trees
- Fast to find
- Backup in cloud and in hard drive

However, before getting into these, let us see why we need a file system at all.

#### What files do I write

When I was at undergraduate, I finally gradually learned the importance of keeping notes of the course. Before then in high school, I did take notes but they lost my interest once finished written. However, in my college I found the difficulties of keeping knowledge in mind. More likely it is due to the explosion of amount of knowledge rather than meself being older. 

You soon find a paper note is annoying, 

- It's hard to revise since no space are left
- It's heavy to bring everywhere especially when half of the notebook is empty
- Your handwriting is disgusting. 
- Paper are weak: they become soft, saturated and someday not capable to bear any information 

Then you wanna be a cool geek taking all your notes electronically, but later you found it ridiculous

- By no means you can type that fast
- It's not intuitive, especially when a sketch should explain all things where your mouse and keyboard looks useless

Wait, why not using ipad and apple pencil? 

- It needs time to load every time you flip through and try to check anything
- If you want to look at a pdf and take note simultaneously you feel it ridiculous to switch back and forth. 

And what's more, your electronic products get broken even faster than your high school paper note. If you are old enough to hold a electronics for a few years you will know what I'm saying. 

Thus, I developed a way to solve all these drawbacks: 

- Take notes on A4 paper (from printers anywhere) to catch up in courses, or think intuitively on some haunting problems. 
- Punch holes in these A4 papers and collect them by little rings (check KW-trio). Do that after the paper is filled with scratches, so that you don't bring blank paper, and it's always comfortable to write on. 
- Reorganize and summarize it to Markdown files so that easy to check later. 
- Use Zotero+Nutshell Netdisk to store the notes in cloud (so you can check it on any library computer once it has Zotero downloaded. )
- Ipad+goodnote is used for writing homework. 

That means, I'll have bunch of files containing my notes and I do check them for concepts or formulae. That makes sure you grab the right thing immediately without adding too much burden to your memory. 

#### Find your file

Once your file is too much, you found it hard to find, even if you establish file trees elegantly, since it's too many layers. The easiest way is "Spotlight" for Mac or "Windows Search" for Windows. However, they don't always show the most wanted result in the front. That urges me (to urge AI) to write myself a search tool.

The result is, basically you press a shortcut to call the tool, input part of the name of the file wanted, then it quickly matches it and automatically open it for you. It's not hard to accomplish, just a paragraph of bash and a app UI using Automator in MacOS. I (followed AI's advice to) name it QOpen. 

#### Clound settings

As said, use Zotero + some net disk. Not only for the papers, but also your notes, even codes. However, Zotero keeps each file in a separate folder. So I can't create symlinks of certain folders to where QOpen searches. At the same time, I don't want to symlink the whole Zotero folder, otherwise QOpen will search inside too huge a folder. 

Thus, I will create a "file item" in Zotero but in its folder hides several files. The "file item" now essentially is a "folder item". However, then I still need to create symlinks one by one in my original folder. 

> Don't change the original name of Zotero files. Otherwise next time you double click the item it reverts the folder all the way up to the day you changed the name. 

 