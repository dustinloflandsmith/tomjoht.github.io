---
title: "Reader question: Am I specializing too much by limiting my focus to docs only?"
permalink: /full-stack-technical-writer-versus-more-specialized-doc-role/
categories:
- technical-writing
keywords:
bitlink: https://idratherbewriting.site/fullstacktechwriterdebate
description: "A reader asks whether he should be focusing not only on writing good developer docs but also building out doc portals and marketing material &mdash; in other words, being more of a 'full-stack' technical writer. This question taps into the dilemma between being a specialist or generalist."
---

A reader recently asked,

> In a recent job interview, in addition to creating API documentation and other technical content, the company wanted me to put together the documentation portal (to resemble Twilio's), write white papers, and work on marketing collateral. I felt my strong suit was in the technical side of reading code and writing about APIs and user guide type documentation. Was I wrong to specialize in documentation only? Should I also be expanding my focus on doc portal tooling and marketing collateral to stay marketable?

The dilemma between being a specialist versus a generalist is a problem I explore in depth in [Principle 11: Be both a generalist and specialist at the same time](/simplifying-complexity/both-a-generalist-and-specialist-at-same-time.html). Many employers want this "full-stack" technical writer, and though they might list all of these requirements in job ads, it's highly unlikely that they will actually find someone who is (1) an API doc-writing ninja, (2) a UX developer who can put together a compelling doc portal, and (3) a knockout marketing copywriter who can sell the benefits of a product through white papers, ebooks, and other campaigns.

Even if you could do all of this, would you have the bandwidth for it? Part of me says yes, and part of me says no. It sort of depends on how complex the product is. The part of me that says yes feels that these activities all build on the same knowledge base, so you're most suited to doing all of these activities yourself. Who better to design the doc portal than the person creating the information for said portal? Who better to tell the product's story than the one documenting the product?

To simplify the doc portal, you might consider going with [Stoplight](https://stoplight.io/) or [Readme](https://readme.com/). Or hire [Pronovix](https://pronovix.com/) to build the portal. Or even [Document360](https://document360.io/) or [Confluence Cloud](https://www.atlassian.com/software/confluence). You don't have to hack this out from scratch. Lots of companies do, for sure, but they might have more resources for it. Even Sendgrid, which is now a Twilio company, [uses Stoplight for their API reference content](https://sendgrid.com/docs/api-reference/). And Box [uses Readme.com](https://developer.box.com/). At the most basic level, doc portal is just a landing page that has links to your other docs. For example, here's the [doc portal for AWS](https://docs.aws.amazon.com/).

{% include ads.html %}

Even if you didn't want to tackle the doc portal, you'd have to implement some other tooling. For example, suppose you wanted to use Madcap Flare, or Paligo, or OxygenXML &mdash; there's going to be some time and tools development required, whether it's creating stylesheets or defining publishing workflows or learning the right XML schema for docs.

However, if by "doc portal" they mean a site with a comprehensive search that has faceted filtering, a fully-featured blog, a forum module, and more all seamless branded together, then that's more full-scale. At any rate, sometimes companies have a lot of budget for solutions like this (even if they don't have budget for hiring), so explore what's possible. Some technical writers act as product managers for third-party companies that develop out the solution. When I worked at a company called Badgeville years ago, my manager worked with a third-party company building out the doc portal in Drupal. She knew exactly what the doc templates needed to look like (based on her research), so she was well-suited for the role. She wasn't expected to actually create the Drupal site herself. So clarify expectations around the doc portal role first before deciding whether this effort expands beyond your scope.

Re the marketing role, I also think that tech writers are well-suited for this. Docs frequently omit the high-level story, the kind of narrative conceptual content that takes a user through their whole journey, or which connects with that user's story in more powerful ways. (For more on story, see [Principle 8: Align the product story with the user story](/simplifying-complexity/articulate-invisible-stories-that-influence-action.html).) I frequently hear feedback that we need more of this high-level information in our docs. One of my goals is to more seamlessly blend marketing and documentation content. The notion that marketing tells the "why" behind the product while documentation explains the "how" is an artificial distinction. Developers are turned off by marketing shenanigans. As a technical writer, your closeness to raw technical information and your preference toward plain language might make you much more suited for marketing to a developer audience.

That only leaves the API documentation and other technical content, which is a task that you're already ready to knock out of the park.

Let's go a bit deeper here with the question about playing multiple roles. About 10 years ago I wrote a series of posts called [From Overlooked to Center Stage](/2010/04/11/if-youre-in-atlanta-next-week-be-sure-to-check-out-currents/). In it, I explained how I started wearing more and more hats as a technical writer &mdash; doing screencasts, usability testing, wiki management, QA testing, and more. It was empowering, but then I hit a crisis point with bandwidth. In [Crisis Point: Problems with Multiple Roles](/2010/04/24/crisis-point-problems-with-multiple-roles-overlooked/), I explained:

> I knew that I had been sloppy and careless in a lot of the help topics, and I just hadn't had the time to go back and carefully review all the content for the upcoming releases like I wanted to. I was being stretched in so many directions, it was hard for me to do what I was initially hired to do: create help material. At times I would refuse to answer simple emails because I knew it would take me out of my rhythm and make it harder for me to get my work done.
>
> ...
> Finally, what did playing these other roles ultimately do for me? It seemed that at the end of the day, I was still evaluated on the help material I produced, not the number of bugs I logged, not on the number of design suggestions I championed, not on the number of users I helped. Those seemed to be invisible efforts that, although appreciated, ultimately remained somewhat invisible. But you could hold a manual in your hand. You could see an online help system. You could watch an instructional video. And you know who produced the material, and you can evaluate the employee based on those products.

I hit a burnout point. I wasn't building a doc portal, but I was wearing multiple hats in other ways with support and QA and usability. Was I wasting my time, especially given that at the end of the day, I was only being evaluated on the documentation deliverables I produced?

I decided that no, wearing multiple hats wasn't *diluting* my ability to write docs. Instead, it was *enhancing* my ability to write docs. In [Epiphany: Cross Pollination](https://idratherbewriting.com/2010/04/25/epiphany-cross-pollination-overlooked/), I explained:

> As I was writing one day, I realized that my extension into these other areas had made me a much faster, more efficient writer. It made me more aware. From my interactions with customers, I could better imagine personas. Often after writing a topic, I would picture that frazzled user who had me on speed dial and wonder if he would actually get what I was writing. I could think about specific users, like the people in Europe who traveled constantly, or the executives in audiovisual, or the mission presidencies in Russia. I could step inside the heads of the users better because I had actually interacted with them. The questions they would ask would naturally be on my mind as I wrote documentation.
>
> The bugs I was logging integrated me with JIRA. I knew how to look and see if bugs and quirks would be fixed or not. I learned how to speak and communicate with developers. I could also see bugs where QA engineers could not see them because I brought the perspective of documentation as I explored the application. I could anticipate possible problems on different screens in ways QA couldn't. And as I applied the tools of documentation to my bug logging, adding screenshots with callouts and videos, I introduced QA to new methods that they adopted.
>
> As I created scripts for my videos, I began to see how the dry, technical language in my help topics contrasted with the lively, conversational voice I had to implement in the video scripts. As I wrote, I often imagined myself speaking to the user in a video script. It's amazing how conversational that helped me to be.
>
> Because I was more of a presence in meetings and outside my cube, people trusted me more. They more freely communicated with me more to relay problems and issues. I could be a better wiki manager because I was accustomed to interacting with others, giving guidance and feedback in tactful yet assertive ways.
>
> All of these ancillary activities weren't detracting from my ability to do my job. Instead, they were enhancing my ability to do my job. I was becoming a better technical writer not in spite of these other roles, but because of these other roles I filled.
>
> Given this cross-pollination effect, I openly welcomed the new roles I would play. Each new role would give me a new perspective, a new pair of eyes. And the more I could see the project from different perspectives, the more of an asset I would be to the team and to the success of the project.

I wrote that "From Overlooked to Center Stage" series in 2010, in preparation for one of my first keynotes at a conference called STC Atlanta Currents. Looking back at the jobs I've had over the years, playing multiple roles has been a constant in nearly every situation.

The challenge is always bandwidth. I frequently feel that I could do so much more than I'm currently doing, if I could only find more time to do it. I want to dive into doing more user testing with docs, comb through support logs, join product meetings to influence design and roadmap decisions, create end-to-end tutorials, build out sample apps, collaborate on ebooks and white papers, explore analytics in detail, and more. But I don't have time.

So the question becomes this: Do you reduce and simplify your scope and role so that you can "do few things but do them well" (to quote a line from a [St. Francis movie](/2008/07/23/tips-for-distributing-the-workload-among-your-team-answering-a-readers-question/))? Or do all of these "extra" activities actually empower you to write better documentation, in ways you couldn't achieve without the extra-curricular activities?

There's a Russian proverb I have taped at the corner of my monitor that says, "If you chase two rabbits, you will not catch either one." But you could make the argument that if you chase two rabbits, you'll begin to see the general patterns that rabbits follow, and you will get a better sense of their behaviors and characteristics, and then you will be more likely to catch a single rabbit when you chase it.

Coming back to your initial question. Should you gladly throw yourself headlong into several directions at once: writing API docs, building doc portals, and creating marketing collateral? Surely, just writing great developer docs probably requires a lot of time ramping up on programming languages and technical platforms. I don't have a great answer here. There are tradeoffs to being both a generalist and specialist. Fortunately, the industry is wide and diverse enough to accommodate both approaches.
