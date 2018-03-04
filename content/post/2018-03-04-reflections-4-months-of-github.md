---
title: 'Reflections on 4 months of GitHub: my advice to beginners'
author: Suzan Baert
date: '2018-03-04'
slug: reflections-4-months-of-github
categories: []
tags:
  - Git
---

Yesterday marked my four months membership of GitHub. Back then, I had seen many GitHub repos pass by after joining Twitter a few weeks earlier, and I wanted to star some of them to find them back more easily. It took another 23 days before I actually committed something myself. 

![](https://github.com/suzanbaert/BlogFiles/blob/master/content/images/180304_GitHub_Contributions.png?raw=TRUE)

Now, four months later, I use GitHub (private) and GitLab (work) as good as daily, and I have inspired others to start using it. Whether you are collaborating or just using code on your own, getting on GitHub is worth it: it gives you version control, it helps others to see your code and learn from it and it gives that 'open source feeling' that everything is out in the open: your data and data manipulations; everything is visible and reproducible.

I got some valuable advice when I just started Git, and then there is some advice I wish I got immediately.  

So to whom it may concern:

<br>

### 1. If you can code in R, you can code in Git's command line. Full stop.
I started by using the Rstudio Git integration, which occasionally did very weird. I felt like I had zero control over what was being added and what not, and I wasn't sure when it was working and when not. As much as I appreciate what Rstudio is doing,  I can only repeat the advice I got: use the Git Bash Command Line. My take on it now is no different: if you can code in R, you can code in Git. Full stop.

Especially when you are working alone on a repo, it takes about 3 commands to have full control over what is happening, and from there you can slowly add to your vocabulary. I made a cheat sheet that at the start only contained a few commands, and I kept building it along the way whenever I had a particular question or problem. [You can find the first part here actually](https://github.com/suzanbaert/Resources_and_Bookmarks/blob/master/GIT_01_Basics.md). By now, I only occasionally have to look anymore, but it's there when I need it.

Unsure where to start? I loved [Corey Shafer's Youtube introduction to Git](https://www.youtube.com/watch?v=HVsySz-h9r4).


<br>

### 2. Gain confidence by learning Git on a bogus Git repo
It's unavoidable that at some point you will go *"oh nooooo!"*. My first one was on a repo of my blog. I had just posted my second post (first time on a new branch!) and somehow ended up with merge conflicts when I was trying to merge that branch. Trying to fix those way too fast, and not really knowing what I was doing, I clumsily got myself in a `detached head state`, and that's when the panic really started.

The mistake was that I was experimenting with more advanced things on a repo that actually mattered. Straight after, I made a bogus Git Repo to experiment with. A safe repo where it did not matter if the whole thing fell apart (and it did).
It didn't even contain code, mostly .txt and .md files. At the very start I literally wrote text that belonged to a commit so I could see it disappear or reappear. Apparently at one point I resetted everything back to commit number 2...

![](https://github.com/suzanbaert/BlogFiles/blob/master/content/images/180304_bogus_git_repo.PNG?raw=TRUE)

 You can even make two clones of the same repo, or make changes via the GitHub website, to simulate what would happen with collaboration.

So the next few hours I was busy resetting, reverting, branching, merging and checking out until I felt that I really got the hang of it. Even now, before trying something new the first time, I use my bogus GIT repo. It's a massive confidence boost, because this way you *know* what will happen when you type on those commands on an  repo that does matter. It's not a 100% guarantee, but it does help.

<br>

### 3. Make those README files for future-you, and get a good text editor.

Something I'm not doing as often as I should: make your own documentation. Make sure future-you remembers what was going on.

And to make that easy on yourself: get a good text editor. I used a few that didn't fully do what I wanted it to do, and now got [Atom](https://atom.io/), an open source text editor made by GitHub actually. It turns any folder into a project, so you have all those files together and it has a preview function for markdown, so I have less additional commits trying to fix a line or a heading.   
It's so useful that I'm converting all my cheat sheets to markdowns in a special repo, so I have them available from anywhere. 

The nicest Atom-surprise came this week, along with a merge conflict: Atom has a really nice feature for merge conflicts. It highlights them so you find them easily, and gives two buttons to select the code you want to keep. Love it!

![](https://github.com/suzanbaert/BlogFiles/blob/master/content/images/180304_Merge_conflict_highlighting.PNG?raw=TRUE)

<br>

### Final thoughts

To "celebrate" my four months on GitHub, I yesterday read the [Git In Practice book by Mike McQaid](https://github.com/GitInPractice/GitInPractice#readme) - which is brilliant by the way! I learned even more things, but most importantly, it finally clicked in my mind how companies are using Git. Just having a feature branch and merging it into master didn't seem like a brilliant work flow if a few people working on the same repo. I already get into a few problems because I work on most of my repos from more than 1 PC, imagine if a whole team is working on them in parallel! His explanation of working strategies in chapter 13 on merging and rebasing finally put the light on in my head.


<br>

### Resources

My advice: start with Corey's video, then Jenny Bryan's book. Get help along the way with Atlassian tutorials, and after you feel somewhat confident, read Mike's book to make things really fall into place. Oh, and get yourself a bogus git repo.

+ [Git in practice, by Mike McQuaid](https://github.com/GitInPractice/GitInPractice#readme) - Highly recommended but perhaps not as complete novice.

+ [Atlassian GIT tutorials](https://www.atlassian.com/git/tutorials/git-stash)

+ [Youtube tutorials by Corey Schafer](https://www.youtube.com/watch?v=HVsySz-h9r4&list=PL-osiE80TeTuRUfjRe54Eea17-YfnOOAx)

+ [Happy Git with R, by Jenny Bryan](http://happygitwithr.com/) - last but not least, Jenny's explanation is excellent for beginners. I also owe her a big thank you for helping me set up with multiple Git SSH keys so I could work on both GitHub and GitLab on my work PC. 
