---
layout: post
title: "Explaining what Cloud Delivery Services to a 6-year old"
date: 2020-05-20 18:00:00 +0530
categories: tech
---

# Explaining what Cloud Delivery Services to a 6-year old

![image](https://miro.medium.com/max/1400/0*CQoQi0uZfKusP4UM)
<p style="text-align: center;">Photo by <a href="https://unsplash.com/@floriankrumm">Florian Krumm</a> on <a href="https://unsplash.com">Unsplash</a></p>

An easy way to revive a flagging dinner table conversation of computer science enthusiasts is to bring up the topic of cloud delivery services. Even Erlich from Silicon Valley couldn’t stop himself from hating on the phenomenal charges of AWS. Have you ever wondered what these might be? Have you always just nodded along to words like IaaS, PaaS and SaaS so that I didn’t look dumb?

This 5-minute blog post is dedicated to all those who to learn cloud concepts but in a simple and easy manner.

Let’s say that your end goal is to go from point A to point B.

You would then have three choices, you can either choose IaaS, PaaS or SaaS.

Choosing IaaS would be analogous to buying a car. While buying a car, you look for all the specs, the colour of the car, the interior design of the car, and would also do a lot of research before buying one: you would go through reviews, ask your friends about their experience using one and take the models for a test drive. After all this hassle, when you do decide on the car, you would buy it, after paying for it and then get to drive it. Here the car is the ‘infrastructure’, you driving it is ‘using it’ and when you for it, it is ‘service’. This entire analogy would resonate with going on AWS, renting an EC2 instance and spinning a Windows machine.

On the same grounds, PaaS is analogous to renting a car where you do not have to do any prior research on specific specs but there are few already bought cars that come with built-in specs. Say for instance, you are renting one from Zoom cars for a little trip with your friends. You would just pay for it and then get to drive it. Here the rental car is the ‘platform’ and everything else stays the same as the previous example. This would then map onto the example of using AWS BeanStalk where you tell what you want, and it automatically runs an instance and downloads all the software you want.
Lastly, SaaS, can be considered as a taxi, say Ola/Uber where you don’t even get to drive the car but are using someone else’s service to go from point A to point B. Here, you are using someone else’s ‘Software’ and rest everything stays the same. This would be using Microsoft 365 services online.

A little look into the specifics might give us a more concrete idea:

**1) IaaS:** A third-party provider hosts hardware, software, server, storage and other infra components on behalf of the user which is mostly used to replace what you have in the data centres like storage and compute services.

Advantages of using one would be elastic Scaling, expenses shifts from capital expenses to operational expenses, you get to avoid buying hardware and software(YAY!), supports public, private and hybrid deployment models

Examples would include AWS, Azure, GCP

**2) PaaS:** It’s a cloud version of app dev, deployment and hosting of apps which provides complete development, testing and deployment platforms and helps reduce application development and deployment cost. Also reduces the complexity of development and testing by placing the developer in a limited environment.

Supported by most IaaS cloud providers, including AWS, Google and Microsoft. Eg. Google App Engine, Microsoft Azure and AWS BeanStalk

<p style="text-align: center;">
Why can’t we use PaaS instead of IaaS?
If you have existing legacy applications already running on your private servers, moving them on PaaS will be difficult because let’s say you want to use AWS as PaaS then as you can see from the above diagram, you will be using the database provided by AWS. This means you will need to change your code to use AWS SDK which can be a tough task.
</p>

**3) SaaS:** A third-party provider hosts app software on behalf of end-user which Removes the need for organizations to install and run hardware and software within their own data centers, and eliminates the waves of hardware and software acquisitions as well as provisioning, maintenance and software licensing. It is mostly used to replace enterprise applications like CRM. It supports both desktop and mobile computing, and there is no need to spend a large amount of cash on software and hardware.

Another really great analogy that we found off of the internet and that we believe would resonate well with all our readers, is:
![image](https://miro.medium.com/max/1400/1*KtNxFJwiP5JTQ9P_gx4MuQ.png)

We hope you liked reading our blog post! Let us know in the comments what you would like to hear about in our next informative post!

# About The SCRIPT Group

We are a tech-enthusiastic community of students. We conduct regular tech events to keep our fellow members up-to-date with the latest tech around the world!

Join us on [telegram](t.me/thescriptgroup) to get started.