---
layout: post
title:      "Regex to the rescue"
date:       2020-05-10 09:12:26 -0400
permalink:  regex_to_the_rescue
---


So this passing week was the first major solo project of my coding life. We had to come up with a CLI application that utilizes nokogiri to scrape data from a website and incorporate those datas into ruby objects that we intended to use in our programs. Without the spec files of the labs and those nice instructions or README, I kinda felt like in hot water in the beginning. But with the helpful little hints, the videos and seemingsly hundeds of those error codes, it's finally done. As I was struggling , I found out how helpful and collaborative the software development community is. It's amazing to see that there is every kind of solutions for almost every kind of problems out there. We just need to know how to find it  and when time comes and if we are in a state where we can contribute, we should be willing to help back. I am not sure if it happens to everyone but when I was doing the project I was so focused  and stressed on the big picture that I started messing up the little things. After countless hours of struggling and staring at the screen, I was practically making mistakes with the simple tasks also. That goes to show that how important it is to take breaks in between coding. One of the problem I was facing when I was building my CLI app was to remove stubborn whitespaces from datas that I was scraping from the website. I tried implementing .chomp/.strip but didnt seem to work. So I turned to google and it led me to the stack overflow where I found this handy little snippet that uses gsub and regular expression to find whitespace at the beginning of the string. 
```
string.gsub /^\s+/, ""
```
It's also worth to note that there is ruby string method that removes the whitespace from the beginning of the string too although I've never used it prior to this project. 
```
string.lstrip
```
These solutions magically took the problem away and made me interested to learn more about regex. I am still trying to learn about it but it seems really powerful and elegant way to solve problems. What do you guys think about this regex? If anyone has a suggestion about how to understand and master the skill of using regular expressions, please comments below!
