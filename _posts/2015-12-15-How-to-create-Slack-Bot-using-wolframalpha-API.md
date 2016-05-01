---
layout: post 
title: "How to create Slack Bot using Wolframalpha API"
date: 2015-12-15 12:00:00
header-img: "img/slack.jpg"
author: "Vikesh Tiwari"
catalog: true
tags:
    - Slack
    - Bots
    - Technology
    - open source
---

Hello everyone,

It's been four days, my exams just got over. During exam time my thought process reaches at its peak and I get so many project ideas, I feel like "I should try this and this. I should start coding right now. What am I studying!? It's of no use lets create something and fuck this!" LOL :D 

Ok I'll write all my thoughts someday later. Let's come back to topic. I read a thread on reddit about Wolframalpha API and I decided to try my hands on it. I created two Bots using Wolframalpha and both work very nicely see some of the best tweets from [L](https://twitter.com/The_L__) . There is an issue with Wolframalpha API it allows only 2000 API calls in a month, you need to take their paid plans if you make heavy usages.

This tutorial is about How to create your own Slack Bot using Wolframa API. I created one but you can not use it directly as it uses my App-Id and can make only 2000 API calls. (Obviously I'm not going to spend my money)

You need basic knowledge of python to create your own Bot.

Steps to create Slack Bot
=========================

## Step 1: Basic Stuff

- [Dev Wolframalpha](https://developer.wolframalpha.com) 
  - Go to developer Wolframalpha and create your account.
  - Go to [My apps](https://developer.wolframalpha.com/portal/myapps/index.html)  section and click on Get an AppID.
  - Note your AppID. You will use this AppID to make calls.
- [Heroku](https://www.heroku.com) 
  - Go to Heroku and create an account there. Heroku allows you to deploy maximum 5 apps on the cloud for free.
  - Once you create your account there. Go to [Dashboard](https://dashboard.heroku.com/).
  - Click on the '+' sign on the top right, create a new app. 
  - Write the name and click on Create App.
  - You will be redirected to your app page. Click on Connect to dropbox. I'll tell you the reason why we are choosing dropbox to for our code hosting.

## step 2: Changes in Code
 - Download my repo in [Zip](https://github.com/vicky002/slack-TheL/archive/master.zip)  or [fork](https://github.com/vicky002/slack-TheL#fork-destination-box)  it to make changes on git in the future.
 - Files in your directory
 	- LICENCE : This is my LICENCE file.
 	- `Procfile`: This is a startup file and tells what is first step when we deploy our app on the cloud.
 	- `app.json`: It is a manifest format for describing web apps. It declares environment variables, add-ons, and other information required to run an app on Heroku. This document describes the schema in detail.
 	- `app.py`: Main part of your project.
 	- `config.py.example`: `config.py` files store variables and other stuffs which is used in your project (Flask).
 	- `requirements.txt`: This file specifies Python Module dependencies. All the required modules would be downloaded first while deploying your app. Read more about it [here](https://devcenter.heroku.com/articles/python-pip).
 - Changes to be made
 	- Open your project click on `config.py.example` file and add your APP_ID in single quotes.
 	- Change the name of the file from `config.py.example` to `config.py`. 
 	- If I upload my `config.py` file on GitHub, anyone can use my APP_ID to make calls. That's the reason naming it as `config.py.example` :p

## step 3: Upload your code on dropbox

 - open your [dropbox](https://www.dropbox.com)  account.
 - If you have connected your account to dropbox as mentioned in step 1. Open this [link](https://www.dropbox.com/home/Apps/Heroku).
 - You'll see a folder with the name of your app on [heroku](https://dashboard.heroku.com/) .
 - Open that folder and upload all your files there.

## step 4: Deploying your app on Heroku

 - Open your Heroku [Dashboard](https://dashboard.heroku.com/).
 - Click on your app and then deploy.
 - In deploy tab, in Deploy changes section. Write `commit` and click on Deploy.
 - This will download all the app dependencies. If everything is fine, you will see a green tick and your deploy is on the cloud!

## Step 5: Integrate it in your team

 - Open your slack. It should be like `{your_slack_url}/home`.
 - Click on Integration in the uppper left section.
 - Click on Configured Integrations.
 - click on Add next to slash Commands.
 	- Command : `thel` [If you want to change this check explanation of the code below]
 	- URL: `{your_herokuapp_url}/thel` [This can be changed see, code below]
 	- Customize name : Give it some name. I gave it `The L`. 
 	- For the **Autocomplete help text**, check to show the command in autocomplete list.
	- Description: `The Genius L, is now in slack to answer all your queries` OR [anything you want to write].
	- Usage Hint: [search query]
	- Descriptiive Level: Search Query

## Step 6: All Done!
 
 - Open your slack channel and type `/thel` or `[your command]` and type Query.
 - Everything is working fine you will see the result. 
 - Try basic Queries first for the testing purpose, it will give instant response.
 - Congratulation you just created a new Bot for your own Team!! Have fun! :beers:


Explanation of the Code
=====================

I already explained usages of the files in the directory. I created this Bot using [Wolframalpha Module](https://pypi.python.org/pypi/wolframalpha)  and [Flask](http://flask.pocoo.org/)  framework. You should know working with python modules and all the syntax to understand the code.

Here is the explanation.

<script src="https://gist.github.com/vicky002/78ed775802ba1666b6a2.js"></script>

Hope it helps!


Please comment below for the issues related to the post and anything related to My bot Please use the [issue tracker](https://github.com/vicky002/slack-TheL/issues) to report any bugs or file feature requests.

This is my second post, I have thought of writing one post in a week. If you're interested in reading my posts, you can [leave your email here](http://eepurl.com/bIgxHz) (expect one mail in a week) :) .



