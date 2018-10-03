---
title: "Tech comm trends: Providing value as a generalist in a sea of specialists (Part V)"
subtitle: "Part V: User knowledge and understanding"
categories:
- api-doc
- simplifying-complexity
- writing
keywords:
weight: 5
tags: series_trends_specialist_generalist
series: "Tech comm trends: Providing value as a generalist in a sea of specialists"
summary: "Specialists often lack user feedback to guide and inform their decisions. This is an area that technical writers can provide value, especially in helping identify problem areas in the user experience."
date: 2018-10-02T03:13:38+00:00
published: false
---

{% include series/seriesTagGeneralistSpecialists.html %}

## Identifying where the problems are

Another gap with specialists involves understanding users &mdash; their experience of the product, their feedback, their successes and failures. Generally, engineers are sequestered in their own spaces, isolated from the user experience. By understanding users and then relaying the user experience, you can help provide essential, guiding information to project teams.

Some academic research indicates that identifying gaps and errors in docs can be one of the main contributions generalists can make. In an article titled [How API Documentation Fails](https://ieeexplore.ieee.org/document/7140676/) (published in [*IEEE Software*](https://ieeexplore.ieee.org)), authors Martin Robillard and Gias Uddin surveyed developers to find out why API docs failed for their users. They found that most of the shortcomings were related to content, such as content that is incomplete, inaccurate, missing, ambiguous, fragmented content, etc. They summarized their findings here:

<a href="https://ieeexplore.ieee.org/document/7140676/"><img src="https://idratherbewriting.com/learnapidoc/images/whyapidocsfail.png" alt="Reasons why docs fail for developers"/></a>

The problem, they explain, is that the very people who can fix this content are usually fully engaged in development work. Robillard and Uddin write:

> Perhaps unsurprisingly, the biggest problems with API documentation were also the ones requiring the most technical expertise to solve. Completing, clarifying, and correcting documentation require deep, authoritative knowledge of the API’s implementation. This makes accomplishing these tasks difficult for non-developers or recent contributors to a project.    
>
> So, how can we improve API documentation if the only people who can accomplish this task are too busy to do it or are working on tasks that have been given a higher priority? One potential way forward is to develop recommendation systems that can reduce as much of the administrative overhead of documentation writing as possible, letting experts focus exclusively on the value-producing part of the task. As Barthélémy Dagenais and Martin Robillard discovered, a main challenge for evolving API documentation is identifying where a document needs to be updated.  

In other words, simply identifying the gaps in the documentation can provide a huge value for the engineering team. There are potentially hundreds of pages of documentation. How do you know where the problems are, where users are getting stuck, where steps are missing or inaccurate?

The developer authors aren’t going to routinely review the content in meticulous ways. They are mostly blind to any questions or shortcomings users might experience. If tech writers can identify these gaps (even if they can’t write the content to address the issues themselves), this mere identification can provide tremendous value to engineering teams.

### Doc feedback buttons

There are a variety of ways to gather this feedback and relay it to the appropriate engineering teams. One of the easiest examples is the embedded feedback button.

On our docs, we added a “Submit Feedback” button directly below the title, like this:

<figure><a href="https://developer.amazon.com/docs/fire-tv/getting-started-developing-apps-and-games.html"><img src="/images/submitfeedbackbuttonfiretvdocs.png"/></a><figcaption>Users can click Submit Feedback to provide their comments</figcaption></figure>

We wanted the button to be unmistakably visible. In other experiments, we had the button off to the sidebar but most people simply missed it.

The feedback form is pretty simple. It looks like this:

<figure><a href="https://amazon6.qualtrics.com/jfe/form/SV_6DzfbuTrUVlOaCV"><img src="/images/docfeedbackformquestions.png"/></a><figcaption>This is the feedback form -- it's simple and provides a mix of structured and freeform responses.</figcaption></figure>

The form is just a survey. On average we get only a handful of responses each week, but the responses are usually worthwhile. They identify gaps or other problem areas that we otherwise wouldn’t realize. Since we work with a lot of doc sets, not all of which we directly authored or own, when we receive doc feedback, we create an issue for it in our issue tracker and assign it to the appropriate engineering team to address. In this way, we don’t always play a direct role in authoring the content ourselves but we do help identify problem areas and connect engineers with those problems.

### Surveys at select milestone events

Besides embedding visible feedback forms on doc pages, here are a couple of other key strategies. When someone completes a milestone, specifically, when they publish an app in the Appstore, we want to take the opportunity to reach out and ask them some brief questions, so we send them a short survey.

I just started doing this, but the results so far are good. I gather up the email addresses for developers with recently published apps, and then find out what they found frustrating or noteworthy in their experience.

<figure><a href="https://amazon6.qualtrics.com/jfe/form/SV_1AC66cH1d960hH7"><img src="/images/milestonesurveyforappdevs.png"/></a><figcaption>This is a survey we send out to developers who just recently published an app in the Appstore</figcaption></figure>

Responses to the survey usually indicate higher-level trends, noting the experience overall and frustrations with certain processes rather than calling attention to specific errors or gaps in existing documentation pages.

### Summaries of weekly issues resolved

Another technique we use is a little less common but also has interesting results. Each week, we write a summary of all the issues we tackled during that week. We already do this as a reporting mechanism for our group, but we also send this list of completed issues out to a wider group of people, including field engineers, tech evangelists, marketers, and support groups. The email contains all the tickets we resolved and a two-sentence description of each issue.

<figure><img src="/images/issues_summary_slide.png"><figcaption>Each week we summarize all the doc updates we've made. We send this email to a huge list of interested people.</figcaption></figure>

This weekly email works quite well for letting others know what we worked on, since most people tend to be unaware of what doc updates take place (and when and by whom). The regular communication with the field engineers lets them know who to reach out to with their doc feedback. Since the field engineers are our most important group for receiving doc direction and feedback, we want to keep open the lines of communication and allow information to flow as much as possible.

Documentation is a common intersection point for nearly every group in the organization, since nearly every group uses docs as tools for their job. Some months ago, I depicted this intersection point in a graphic and [posted it on Twitter](https://twitter.com/tomjohnson/status/942867105845723136). This tweet had 73 favorites, 37 retweets:

<figure><a href="https://twitter.com/tomjohnson/status/942867105845723136"><img src="/images/generalist_specialist_intersection.svg"/></a><figcaption>Because documentation is used by nearly every group in the organization, it becomes a common intersection point through which you can gather input from many different intersecting groups.</figcaption></figure>

Marketing uses tech docs in their blog posts, support agents point to it in responses, training uses it in their materials. Product evangelists, field engineers, and even internal engineers all use the documentation, and so on.

{% include random_ad.html %}

If docs are at this intersection point within the organization, we should be able to gather feedback from all of these different groups about the docs. Many of these groups regularly interface with customers, which means they can relay the user experience.

Imagine a scenario where, even in a large organization, everyone knows who writes the docs, which docs they work on, and how to influence change in docs. When you have good communication with these groups, feedback flows in.

## Your reactions and input?

<script>
EMBED_PARAMS = {};
EMBED_PARAMS.surveyID =6324683;
EMBED_PARAMS.domain ="//www.questionpro.com";
EMBED_PARAMS.src ="//www.questionpro.com/a/TakeSurvey?tt=nZzmfCaclpY%3D";
EMBED_PARAMS.width ="100%";
EMBED_PARAMS.height = "750px";
EMBED_PARAMS.border = "hidden";
</script>
<div id="div_6324683"></div>
<script src="//www.questionpro.com/javascript/embedsurvey.js?version=1"></script>

You can <a target="\_blank" href="https://www.questionpro.com/t/PESa9Zc1tU">see the responses (so far) here</a>.

{% include series/seriesTagGeneralistSpecialists_next.html %}