**Bryan 2017**

*What problems can setwd() cause in your scripts and how do RStudio projects address them?* 

Using setwd() means that other people who try to use your code will struggle, potentially leading them to commit crimes such as arson. It's unique to your computer, meaning that if you move anything around or rename it, it will be super annoying for future you and your collaborators. 

*When you call rm(list=ls()), what is removed from your environment? What’s left over that restarting your R session would remove? What’s the keyboard shortcut for restarting your R session?*

All objects are removed from your environment, but there's still a bunch of other stuff that lingers (settings, options, etc). That means that you might think you have everything you need in the script, but actually you're just relying on stuff that's leftover that no one else (including future you) will have access to. It also might mess up someone else's analysis if they open your code on their computer! The keyboard shortcut is Command + Shift + 0. 

**Bryan 2018**

*The basic git commands are commit, push, and pull. Which commands change happen locally (i.e., on your computer)? Which happen remotely?*

Commit happens locally from your computer. Push and pull happens remotely. 

*Why do diffs work for source code (e.g., .R files) but not Word documents (i.e., .docx files)?*

Diffs are the set of differences between versions. Word documents are large binary files and are beyond the reach of Git's automated merging. Diffs are easier to track in .R files. 

*Why is Markdown useful for GitHub repos?*

They can be rendered to other formats, like html, pdf, word, and can incorporate code chunks from other languages. It's also good because it's plain text, but works like an html website. 
