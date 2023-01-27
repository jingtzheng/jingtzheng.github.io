---
layout: essay
type: essay
title: "Questions of Questions"
# All dates must be YYYY-MM-DD format!
date: 2023-01-26
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/question.png">

## My curiosity

As a curious child, I have always asked questions. I would always ask 'why' and 'how' and often jump ahead of the lectures. Teachers would always say "Wait, it is on the next slide! We are getting there." Sometimes, the teachers tell me that they don't know the answer either or you don't need to learn that in-depth. But, as a curious soul, I just had to learn about the topic to the very nitty-gritty bits. Teachers would always mention to me that there are no dumb questions so just ask away! But is this applicable to the real-life when we are actually creating technical solutions for the world?

## A question considered as not as SMART

Over the recent years, Stack Overflow has emerged as the top platform to ask for help on technical questions that programmers are encountering. As programmers range from various skill levels, the quality of questions can also range from bad to good questions. 

The following example demonstrates a question that is not as smart. The author of the question seeks to write python code for certain conditions. 

```
Q: I need help coding this scenario

I can watch another episode before bed:

If it it is before 1 AM and I don't have work or class in the morning

or it is the weekend.

Using python code this scenrio

```

Firstly, 

```
A: datetime and the datetime.timedelta classes are your friend.

1. find today
2. use that to find the first day of this month.
3. use timedelta to backup a single day, to the last day of the previous month.
4. print the YYYYMM string you're looking for.

Like this:

 >>> import datetime
 >>> today = datetime.date.today()
 >>> first = datetime.date(day=1, month=today.month, year=today.year)
 >>> lastMonth = first - datetime.timedelta(days=1)
 >>> print lastMonth.strftime("%Y%m")
 201202
 >>>

```
 
The asker received six possible answers, and he or she was successful in inciting discussion from multiple users. The answers themselves were clear and were devoid of the rumored sarcasm and hostility of “hackers.” Since I myself have referenced this page and found it useful, I can confidently say that it is a good question.

## The foolproof way to get ignored.

While there are decent questions that benefit everyone, there are those one can ask to create an entirely different effect. In the following example, a user asks how he would, in short, create a desktop application with Facebook.

```
Q: Facebook Desktop Notifier

I am a beginner programmer that have never used anything other than what's included in a language.

I am trying to create a desktop application that notifies me anytime I get an update onfacebook. 
How should go about doing this? Thanks in advance.

edit Sorry I was not clear. Is there any way to make a DESKTOP application with facebook?
```

A simple “yes” would have answered the question, but we know that’s not the sort of answer he or she is looking for. Fortunately, someone kindly responded with a link to Facebook’s developer website. The asker should have done more research on his or her potential project. Then further down the road, he or she could have asked more specific and detailed questions that wouldn’t require a thousand-paged response for a sufficient answer.

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.
