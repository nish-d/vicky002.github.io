---
layout: post 
title: "Getting started with Open Source: The Ultimate guide"
subtitle: "Trust me, it's not that hard!"
date: 2016-05-02 12:00:00
header-img: "img/osi-min.jpg"
author: "Vikesh Tiwari"
catalog: true
tags:
    - open source
    - Technology
    - learning
---

Hello! 

After a few, <a href="http://eulercoder.me/tags/#personal" target="_blank">Love, life and personal articles</a>, it's time to write some technical stuff. After my post on <a href="http://eulercoder.me/2016/03/01/Competitive-Programming-or-Development-which-one-to-choose/" target="_blank">Competitive programming or open source development which one to choose?</a>, I received so many emails asking How to start with open source. I wanted to write about this since a very long time so as the title suggests, this blog post is for beginners who want to work on their own projects or contribute to other open source projects. **This is going to be a long post so grab some snacks, take a notebook and make a note of points that you think may help in the future.**  

Before we start, Don't think about: 

*Am I good enough?*
*Will my pull request get rejected?*
*Will my code bring me shame for years?*
*Is it worth the hassle?*

Many people are afraid to contribute to open source because they don't feel up to the task or don't have years of experience or enough in-depth knowledge about something.

Trust me, 
*The first time is **always** the hardest, and once you get started on contributing to open source you will see how easy it is and what are the benefits and rewards.*

You do not need a degree or an invitation to contribute to open source. If you want one, you are hereby cordially invited :).

So let's get started!

# So Vicky, tell me what exactly is open source? 

The term "open source" refers to something that can be modified and shared because its code is publicly accessible. Open source software is 

> *a computer software or application with its source code made available for **free** with a **license** which can be modified, changed and distributed to anyone and for any purpose.*

- **free**: A software is not open source if you need to pay for the source code
- **license**: License provides the rights to study, change and distribute the software. 

Companies make their projects open source which allows developers to stop complaining about the bugs or required features and actually solve them. 

# Ok Vicky. Now I know about Open Source but why should I contribute?

I'm glad you asked this question before we actually start the main part. There are tons of benefits associated with open source. I can write another blog post on benefits of Open source.   

Below are some benefits of contributing to open source.

- Open source is an excellent way to level-up your skills as a developer. It's handy to point to your open source projects and contribution work as an example of what you're capable of.
- It makes you learn more.
- Gives a good impression about you that you work with development because you love it. Love it enough to spend your free time on a free project.
- You help eagerly to make a better software for yourself and others. It gives immense pleasure to contribute to a software which is used by thousands of people.
- This will improve your development skills, more skills' means more opportunity, and by working on projects you enjoy, that opportunity can be more enjoyable too.
- Open source is fun, challenging, and totally worth your time and effort.


# Whoah! This seems very interesting Vicky, tell me the very first step?

Yeah! :) 
The undisputed center of the open source universe is <a href="https://github.com/vicky002" target="_blank">GitHub</a>. Github enables individuals and organizations to create projects, fork them and contribute to it. The very step is to learn about <a href="https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control" target="_blank">Git version control system</a>, <a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git" target="_blank">Installing git in your system</a> and <a href="https://www.atlassian.com/git/tutorials" target="_blank">know about basic git commands</a>. You can also try this <a href="https://try.github.io/levels/1/challenges/1" target="_blank">interactive course on Git</a>. 

**You know what's the best thing about Github?** Anyone can fork any project without approval or oversight from the original authors. Changes can be committed locally, pulled to the parent repository with a code review. Anyone can comment on any single line of code or a pull request. You can use your fork immediately in your project. 

Oh I forgot to tell you about these words that developers use :p. Check what's the meaning of a commit, pull request, fetch, pull, fork, local and parent repository in <a href="https://help.github.com/articles/github-glossary/" target="_blank">Github glossary</a>.


# Vicky, I completed the first step. What's next?

That's good! You're now ready to contribute to open source. There are two major ways you can contribute to open source 

1. Contribute to an existing open source project.
2. Start an open source project.

I am writing on the first aspect - Contributing to an existing project because almost all beginners find this hard. *The hardest hurdle in open source is: The first contribution*. Trust me you may not feel like a super genius, but you definitely don't need to be one to contribute to open source. It's just that first contribution to get you started, then you're hooked. It doesn't have to be monumental or anything. So **what open source project should you contribute to?** The best answer to this question is: ***You contribute to something you use regularly.*** This post is for beginners so I'll take my project <a href="https://github.com/vicky002/AlgoWiki" target="_blank">AlgoWiki- Collection of all CS resources at one place!</a> and will contribute something to it. It's extremely easy to contribute to AlgoWiki, it's just a collection of links. I think, this is a perfect project for you and don't worry I be nice sometimes and accept all pull requests. :p 

After your first contribution, search projects on Github that you use regularly. Read code, install it in your local system and start contributing to it.

# Vicky, I'm excited to contribute to AlgoWiki. Tell me how!

Ohh That's super awesome! So let's get started :). When, you see any big project on Github there will always be this three main files. 

- **README.md**: This contains the description about the project, installation, License, contributors i.e. the summary of the project. 
- **LICENSE**: This contains License and other copyright data.
- **Contributing.md**: This file is for developers who want's to contribute in the project.

### Fork the project:

- Open <a href="https://github.com/vicky002/AlgoWiki" target="_blank">AlgoWiki</a>, click on fork on the top right corner.
<p>
<img src="/img/fork.png" align="center">
</p>
- You can now see AlgoWiki in your profile. 

### Clone that repo in your local machine

- Open Your Github Profile, open AlgoWiki forked repo in your profile.
- Copy Clone Link to clipboard. 
<p>
<img src="/img/clone.png" align="center">
</p>
- Open terminal in your local machine and paste that URL. 
```git clone https://github.com/{your_username}/AlgoWiki.git```
<p>
	<img src="/img/local_clone.png" align="center">
</p>

### Making changes in your local repository

- Read <a href="https://github.com/vicky002/AlgoWiki/wiki/Contribution">Contribution.md</a> file of AlgoWiki. It has all details on how to make changes and maintain section, subsections etc.
- Now add links of article, videos or books anything you that want to contribute. 
- Save those files. 

### Push your local changes to the main repository. 

- Now you already know how to add files, commit and push to the main repo.
	- ```git add file1 file2 file3```
	- ```git commit -m 'commit message'```
	- ```git push origin master```
- You made changes, pushed to master branch from your local machine. This is the first step to create a pull request. 

### Your first Pull Request

For your first <a href="https://help.github.com/articles/using-pull-requests/">pull request</a>, Let the project manager know that you're new and want some guidance to learn how to get into it. It may so happen that they’re too busy to help, if so, move on and find another project. That first contribution is the hardest, you may want some help and coaching. The actual code contribution matters less than learning the process. So find a project or someone who has time and patience to mentor you. 

Here, I know you are contributing for the first time so I'll be kind here and accept your pull requests in AlgoWiki :p and I am 24/7 online to accept pull requests, discuss changes or anything related to my projects. 

- Go create a pull request and contribute to AlgoWiki!
<p>
	<img src="/img/pull_request.png" align="center">
</p>
- One you create a pull request, owner will check everything. 
- If author finds it useful, he will merge your pull request.
- Don't forget to say thanks because this is your first contribution to open source. 

<p>
	<img src="/img/merged.png" align="center">
</p> 

**Once your pull request is accepted, you can check your GitHub profile. See that green square on your heat map calendar, and that streak? Congratulations!! You’ve made an open source contribution!**  

As you contribute to larger and larger projects, you'll get better at learning codebases well enough to track down bugs and add functionality. 

That's how you learn. That's you grow as a developer. And that's how you prove to future employers that you can collaborate with other people and code that's worth sharing!

# What I learnt from Open Source

I have learned so many valuable skills from my time using and contributing to open source projects. I've learned how many different build systems work, different styles of structuring code and files to enhance readability, Swagger for API which I didn't know existed, etc. etc. etc.

#### Job opportunities

You must be knowing about this. Open source contributions matter a lot. I get so many emails from recruiters to my Github email address. And by developing some street credibility on Github, people start paying attention and are interested in what you're working on.

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">When it comes to hiring, I&#39;ll take a Github commit log over a resume any day.</p>&mdash; John Resig (@jeresig) <a href="https://twitter.com/jeresig/status/33968704983138304">February 5, 2011</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

#### Friends

Lots of conversation that start on Github turn into friendships that extend to Twitter. It gets real fun when you meet these awesome people in real life and I'm super excited to meet a few during <a href="http://eulercoder.me/2016/02/27/My-internship-interview-experience-with-Amazon-LinkedIn-BrowserStack-Mozilla-and-Slack/" target="_blank">my internship at Slack in San Francisco</a>. Friends make open source fun and rewarding. 

### Helping others

One of the most rewarding things when working with open source is when someone says something like: “This is amazing!” “Thank you so much!” “It’s saved me so much time!” or “I wish that I’d found this earlier!” **Call to action**: If a project has saved you some time, go ahead and create an issue to simply tell them thanks. (When show copied Github projects in college.)

# Conclusion

If you haven't contributed to open source before, I recommend you give it a whirl. It's fun, it's rewarding, and it's good for your career. If you're looking for a good project to contribute to, remember that

> You contribute best to something you use regularly.

Contributing to open source has been awesome for me! It’s really hard getting started, but once you get over the first contribution, making future contributions is much easier. It’s not all roses. The open source community has its warts here and there. Keep working at it. You’ll do great! Good luck!

So, **Do yourself a favor and move to Github! Your open source contributions will play in your favor!**


PS: You are always welcome to contribute to my projects. Check out my <a href="https://github.com/vicky002?tab=repositories">GitHub Projects</a>. 

If you liked this article, don't forget to share it with your friends. :) 

Oh, <a href="https://github.com/vicky002/vicky002.github.io/blob/master/_posts/2016-05-02-getting-started-with-open-source.md" target="_blank">see a typo</a>?

<div class="container">
<div class="row">
	<div class="col-xs-2"></div>
	<div class="col-xs-8">
<a href="https://twitter.com/share" class="twitter-share-button" data-via="vikesh002">Tweet</a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.parentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>
&nbsp;&nbsp;&nbsp;
<div class="fb-share-button" data-href="http://eulercoder.me/2016/05/02/getting-started-with-open-source" data-layout="button_count" data-mobile-iframe="true"></div>
	</div>

</div>    
<div class="col-xs-2"></div>

</div>

*Special thanks to <a href="https://github.com/nish-d" target="_blank">Nishita</a> for reading drafts of this! She's awsome!! Super cool and amazing!! :D*

You may also like: <a href="http://eulercoder.me/2016/03/01/Competitive-Programming-or-Development-which-one-to-choose/" target="_blank">Competitve Programming or Open Source</a> | <a href="http://eulercoder.me/2016/02/27/My-internship-interview-experience-with-Amazon-LinkedIn-BrowserStack-Mozilla-and-Slack/" target="_blank">My interview experience with Slack, Mozilla, LinkedIn, Browserstack and Amazon</a>
