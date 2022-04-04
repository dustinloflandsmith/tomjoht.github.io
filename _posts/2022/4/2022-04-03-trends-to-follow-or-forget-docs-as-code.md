---
title: "Docs as Code (Trends to follow or forget)"
permalink: /trends/trends-to-follow-or-forget-docs-as-code.html
categories:
- technical-writing
keywords:
rebrandly: https://idbwrtng.com/trendsdocs-as-code
series: "Trends to follow or forget"
jtype: notes_fizzled_trends
description: "This post is <a href='/trends/trends-to-follow-or-forget-intro.html'>part of a series</a> that explores tech comm trends that I've either followed or forgotten, and why. The overall goal is to better understand the reasons that drive trend adoption or abandonment in my personal career. This post focuses on *Docs as Code*."
---

## What is docs-as-code?

*Docs as Code* refers to writing and publishing docs by following the same tools and workflows that developers use to create code. *Docs as code* systems are characterized by several practices:

* Authoring in plain text files (rather than a visual editor), often writing in simplified markup such as Markdown.
* Managing the files using version control such as Git (rather than a database); this might involving branching and merging in a distributed way to a centralized source
* Building the web output using static site generators such as Jekyll, Hugo, or other [static site generators](https://jamstack.org/generators/)
* Initiating the build through command-line configuration from the server (rather than building locally) to allow for continuous integration
* Managing review cycles through the same diff review tools developers use to review code

*Docs as Code* started gaining popularity around 2010-2015 as some developers expressed frustration with heavy, code-bloated [content management systems (CMS) systems](/trends/trends-to-follow-or-forget-wordpress.html) that had grown overly complex, with a lot of unnecessary modules and infrastructure overburdening the simple task of authoring and publishing web pages. One of the early *Docs as Code* developers was Tom Preston-Werner, co-founder of GitHub, who had an epiphany while blogging. He said:

> On Sunday, October 19th [2008], I sat down in my San Francisco apartment with a glass of apple cider and a clear mind. After a period of reflection, I had an idea. While I'm not specifically trained as an author of prose, I am trained as an author of code. What would happen if I approached blogging from a software development perspective? [Blogging like a hacker](https://tom.preston-werner.com/2008/11/17/blogging-like-a-hacker.html)

This epiphany led to the creation of [Jekyll](https://jekyllrb.com), one of the early static site generators. *Docs as Code* approaches grew in popularity in parallel with the rising popularity of [web API documentation](/trends/trends-to-follow-or-forget-api-documentation.html). If you're writing developer docs, *Docs as Code* fosters a collaborative environment between writers and developers with the documentation, whether that collaboration includes authoring, review, or publishing.

For more on *Docs as Code*, see the many posts I've written on my site:

* [Static site generators start to replace web publishing platforms like WordPress](/2015/02/27/static-site-generators-start-to-displace-online-cmss/)
* [Review of Andrew Etter's ebook on Modern Technical Writing](/2016/07/26/modern-technical-writing-review/#static-site-generators)
* [Flat file systems versus database models for help](/2014/11/05/flat-file-systems-versus-database-models-for-help/)
* [Write the Docs Podcast episode 19: Static site generators, with Jessica Parsons](/2019/01/31/static-site-generators-write-the-docs-podcast-episode-19/)
* [Thoughts on docs-as-code after 3 years -- it works!](/2018/07/03/docs-as-code-after-three-years/)
* [Discoveries and realizations while walking down the Docs-as-Code path](/2017/08/23/content-architecture-and-repo-sizes/)
* [Recording of Docs-as-code tools and workflows presentation](/2018/03/09/docs-as-code-tools-and-workflows-denver-presentation)
* [Will the docs-as-code approach scale? Responding to comments on my Review of Modern Technical Writing](/2016/08/01/responding-to-feedback-on-modern-tech-writing-review/)
* [Case study: Switching tools to docs-as-code](/learnapidoc/pubapis_switching_to_docs_as_code.html)
* [Limits to the idea of treating docs as code](/2017/06/02/when-docs-are-not-like-code)

And of course see Anne Gentle's book on the subject, [Docs Like Code](https://www.amazon.com/dp/B08KY82ZSB/), and this [helpful resources page on *Docs as Code* from Write the Docs](https://www.writethedocs.org/guide/docs-as-code/).

As I gathered up these posts, I've realized just how much I've written about *Docs as Code*. That's partly because I was writing about *Docs as Code* as this trend has come out of obscurity and evolved into a common approach in tech comm. If you're joining the ranks of tech comm in 2022 and writing dev docs, *Docs as Code* might now seem like the default approach. It didn't used to be.

{% include ads.html %}

## Why I embraced docs-as-code

I started using *Docs as Code* (specifically Jekyll) back in 2015 when I was working for 41st Parameter (acquired by Experian), and we were looking for a way to get out of Confluence (we were generating PDFs from Confluence pages and putting them in Dropbox for partners). We wanted to build a modern web experience for our docs. We were investigating [DITA](/trends/trends-to-follow-or-forget-dita.html) in part because we also had requirements to build PDF and also version our content. Tools like Jekyll made it easy to generate HTML, but some of the more complex tech comm scenarios required us to figure out our own approach.

I started using Jekyll as a pilot for a specific project. I built a [Jekyll doc theme](/documentation-theme-jekyll/), which surprisingly has since been [forked and starred on GitHub](/documentation-theme-jekyll/) over a thousand times. The pilot project became our standard approach, and the exploration of other systems faded away.

Jekyll suited me well in part because I'm tools savvy, having worked as a [WordPress](/trends/trends-to-follow-or-forget-wordpress.html) consultant creating themes and other implementations for years. I knew HTML, CSS, and JS well enough to do what I wanted. And Jekyll was simple enough that I could gut any web page into a template, pipe content into it using Jekyll's scripting logic, and make the system do what I wanted.

My big breakthrough in building the theme was to create an expandable/collapsible sidebar that generated content from a YAML file. This robust sidebar was missing from most Jekyll blogging templates. Getting it right required me to understand [how Liquid, Jekyll, and YAML worked](/documentation-theme-jekyll/mydoc_yaml_tutorial). Once I did, I could create widgets and templates for virtually anything (I later contributed a [tutorial on navigation](https://jekyllrb.com/tutorials/navigation/) to the official Jekyll docs).

Jekyll's flexibility and open code allowed me to do practically anything. I made my theme links use entirely relative paths, which allowed me to build an output and view it offline. The zip file could be uploaded to any domain or environment (staging, production, or other) and be easily viewed.

I also created a [PDF output](/documentation-theme-jekyll/mydoc_generating_pdfs.html) using [Prince](https://www.princexml.com/). Again, this required some hacking with PDF layouts and custom CSS, but it wasn't something I couldn't figure out with enough tinkering. And I loved tinkering with Jekyll.

When I joined Amazon, a major project we had was to migrate from a CMS called Hippo (a Java-based CMS, now called Bloomreach, rather than one built with PHP) to Jekyll. I'd come in at the right time because developers were engaged in an enterprise-wide effort to migrate off of Oracle databases, and the Jekyll tooling fulfilled this requirement. No one wanted yet another CMS, and with both PHP and Oracle databases off-limits, there weren't that many alternatives. Additionally, hosting sensitive content (such as confidential docs) on third-party servers was also restricted, which also limited our tool options.

Working in dev docs, I discovered that developers loved working with Jekyll because they could script the build workflows into their own, larger build workflows. The dev team ended up building Jekyll's content output and pushing it into another template that they controlled. This resulted in more seamless branding.

On a personal level, when I first exploring Jekyll and tried to figure out themes, I realized that if I wanted to excel in this domain, I should flip my whole world to Jekyll. I didn't want to maintain my blog on WordPress while using Jekyll at work. If I wanted to gain more familiarity and fluidity with both static site generators and version control in the *Docs as Code* world, I figured I should also use Jekyll for my personal blog.

So I made a rather large decision to abandon WordPress for my blog and to use Jekyll exclusively for authoring and publishing content. This shift did achieve my initial aims. With my [API course](/learnapidoc/) I've even built more sophisticated outputs that [include PDF and ebook](/learnapidoc/docapis_formats.html) (both Kindle and EPUB) from the Jekyll source.

## Why didn't I abandon docs-as-code

I didn't abandon *Docs as Code* because it seems to be the right tool when working in developer documentation. I've noticed that even if developers don't write docs in Markdown (because they don't write docs, period), getting them to *review* docs goes much better if you use their same world of tools. Developers often want to see the exact changes that have been made so they can easily check to see what needs review without rereading the entire page. They also prefer smaller changes to review as well, even if there are multiple change requests to evaluate. Reviewing docs in these tool systems works pretty well.

Even as I've changed companies to Google and the toolset is no longer Jekyll, I'm still very much in a *Docs as Code* authoring and publishing system (see this [talk by Riona Macnamara](/2016/07/15/transforming-documentation-processes-docs-as-code/) for more context). Much of the authoring complexity has been abstracted behind the scenes (and rightfully so), but I'm still working in Markdown, YAML, building from the command line, reviewing diffs through the same tools as developers, and more. And you know what? It works.

It seems like every big tech company uses *Docs as Code* in their developer documentation now. Big companies prefer to roll their own rather than go with out-of-the-box solutions, so there are some customizations and unique differences from one company to the next, but most of what I did with Jekyll and Liquid on my blog I can still do with the authoring systems at Google, which includes [Jinja templating](https://jinja.palletsprojects.com/). In fact, the code manipulation is even better than what Liquid offers, since I can create actual [macros](https://ttl255.com/jinja2-tutorial-part-5-macros/) (like functions) and use them even more directly as code.

There's another point worth mentioning for why *Docs as Code* has remained strong: it scales well for authors. You don't have to provision an ever-increasing number of licenses for those contributing to docs. Anyone can get up and running using the same tools they're probably already using for code, and the workflow for creating and publishing content feels second nature because it highly mirrors their existing developer workflows.

## Current status

*Docs as Code* continues to be popular. The preferences for the static site generators, though, tend to be more shifty. Tides have shifted from Jekyll to Hugo, but there's also a lot of fragmentation here with no common standard for the static site generator (for example, Docusaurus, Gatsby, and MkDocs are also popular). The Git workflows also vary a lot from shop to shop.

So even if you've accrued a lot of experience using a particular static site generator and Git workflow for authoring/publishing, if you go to a new company, you might still have to re-learn the approach. Even so, once you convert to this model, it feels odd to even think of working any other way. I couldn't imagine going back to a specific tool with a visual interface, or to a database-based CMS. I've pretty happy with the *Docs as Code* approach. Rarely do I encounter obstacles that I can't overcome. And the minimalist approach with tools also fits a more minimal approach to the web that I think we'll be seeing more of.