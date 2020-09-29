---
title: "A one-stop shop for government staff to learn how to write open-data policies"
description: "The Open Data Policy Hub collects a number of resources related to open-data policies on a single user-friendly website, replacing five different websites."
image: /images/works/policy-hub/policy-hub-home-page.png
layout: page
---

![Home page of the Open Data Policy Hub](/images/works/policy-hub/policy-hub-home-page.png)

## Summary

I created the **[Open Data Policy Hub](https://opendatapolicyhub.sunlightfoundation.com/)** in August 2018, during my time at the Sunlight Foundation. Its purpose was to collect all of our resources related to open-data policies on a single user-friendly website, replacing resources that had been scattered across five different websites.

## Context

In 2015, the Sunlight Foundation got a grant to help cities around the United States pass open-data policies. Through the work on this grant, as well as some previous work, the organization created a number of resources related to policy for open data:
- [Public Policy for Public Data](https://sunlightpolicy.github.io/wwc-site/)
- [Open Data Policy Collection](https://sunlightpolicy.github.io/opendatapoliciesstatic/browse/)
- [Open Data Policy Guidelines](https://sunlightfoundation.com/opendataguidelines/)
- [Open Data Policy Comparison: Best Practices](https://docs.google.com/spreadsheets/d/1ETZuGZBK24J2viZdxmhyIlIKiJuytAu3Bh1ofo_HVBw/edit)
- [Open Data Policy Wizard](https://docs.google.com/forms/d/e/1FAIpQLSe2BeXHF-vkjbfmYRK0dIxYtWyaXUCkgG0a6twAIqRdwJM8dg/viewform)

The problem was, these resources were all on different websites and had different branding. Furthermore, many of them made references to the others, sending users through circles of these different sites. Finally, there was a fair amount of content that was duplicated across sites, sometimes inconsistently.

![Home page of the Open Data Policy Hub](/images/works/policy-hub/policy-hub-predecessors-before.png)

One result of this mess was that we often had to send people an entire email explaining how to navigate all of these resources — a sign of a broken user experience!

## Goal

The goal was simple: to create a single site that would provide everything a person needs to know to create an open-data policy.

## Process

The Open Data Policy Hub was not the product of a single development process. Instead, it was the culmination of several different iterative efforts over the years.

Thanks to the fact that we had already shared most of the future Hub’s content publicly via the separate resources that the Hub would eventually replace, we had already done internal reflection and gotten external feedback on much of the content and many of the features of the site. In fact, some of these individual predecessor resources had already been revised or enhanced several times.

As such, we did not conduct a “blue sky” discovery process. Instead, we took the lessons already learned and used that as the basis for the new site.

In early 2017, I wrote up the first [concept note](https://github.com/sunlightpolicy/opendatapoliciesstatic/issues/80) for the new site.

In terms of branding, one of the key concepts was to have a set of resources that has a collective name yet where each resource can be referred to individually — so we could tell cities to “check out the Open Data Policy Hub” or more specifically to (for example) “use the Open Data Policy Generator” and not “use the policy generator on the Open Data Policy Hub.” Still, we wanted the set of resources to clearly belong to one family even if referred to separately, somewhat akin to a [“branded house”](https://www.ideasbig.com/blog/branded-house-house-brands/) design approach.

![Home page of the Open Data Policy Hub](/images/works/policy-hub/odp-branded-house.png)

Over a year passed by, and while we had the chance to make a number of improvements to the separate resources, work on the unified Hub did not begin in earnest until mid-2018. We started with some whiteboard and paper wireframes to get us thinking about how users would navigate the site.

<!-- future: image of paper wireframes -->

Instead of then creating digital wireframes or mock-ups, I proceeded directly to implementing our concepts on a real live website.

Because I was the one both designing and developing the site, that meant I had the ability to directly realize our proposals in code. I felt that doing this was the most efficient way to simultaneously create something for people to give feedback on and make progress on the actual product itself.

![HTML from the home page of the Open Data Policy Hub](/images/works/policy-hub/home-page-html.png)

In a way, this was embracing the [design philosophy](https://gds.blog.gov.uk/2014/07/18/whats-the-design-process-at-gds/) of the U.K. Government Digital Service: “The problem with [showing people wireframes] is they’re commenting on the picture of the Thing rather than the Thing itself. It’s better to send round a URL and ask people how it works for them.” In my experience too, people tend to be more responsive to real live websites than to mock-ups of websites. (That said, I’m not categorically against creating digital wireframes!)

One important enabler of my fast progress on the site was open-source software. [Inspired by NYC Planning Labs](https://github.com/NYCPlanning/labs-planninglabs.nyc-archive/blob/master/_posts/2017-06-12-cloning-18f-gsa-gov.md), I forked [18F’s website](https://18f.gsa.gov/) — not because I wanted our site to look similar but rather because it already had a [rich set](https://18f.gsa.gov/styleguide/) of features and design components. I figured it would be a waste of our resources to create a new website from scratch.

![Screenshot from the 18F Style Guide](/images/works/policy-hub/18f-style-guide.png)

<!-- [future — image of Planning Labs new site] -->

Thanks to this foundation, a lot of the basic design work was fairly trivial to implement.

Because our primary audience for the website was people who are not already familiar with the subject matter, I tried soliciting external feedback from two different groups of people: (a) subject-matter experts, who could provide an informed critique, and (b) government staff who were looking to create open-data policies, who could provide the perspective of a user. I was successful at the former and not so successful at the latter.

Due to being a small team with limited capacity, we had somewhat of a need to wrap up work on the project for the time being in order to focus on other projects — despite not yet having as much success with potential-user outreach as I had hoped. We [publicly announced](https://sunlightfoundation.com/2018/08/30/introducing-open-data-policy-hub/) the launch of the new site in August 2018. Since then, though, we have been able to make further edits and improvements based on public feedback.

For what it’s worth, we felt pretty strongly that the new site was an improvement over the status quo, and that we weren’t really losing anything by the switch. And, while I wasn’t so successful at targeted outreach to intended users, having the website be public creates a much broader audience of users to get feedback from.


## Result

**[Check out the site »](https://opendatapolicyhub.sunlightfoundation.com/)**

![Home page of the Open Data Policy Hub](/images/works/policy-hub/policy-hub-home-page.png)

The new site now provides much more cohesive design than the disjointed experience of the predecessor resources.

![Before-and-after comparisons of the predecessor resources and their new versions on the Open Data Policy Hub](/images/works/policy-hub/policy-hub-before-after.png)

Since the launch of the site, we have asked many government officials about their experiences with the site and continue to receive positive feedback.

Additionally, by making it very clear and easy for users to navigate themselves through the process of creating an open-data policy, we have saved ourselves staff time.

One random thing that I’m happy about is the design and functioning of the Open Data Policy Generator. On the front end, the user sees a form that looks just like the rest of the site. But when a user submits the form on this site, their submission data is then passed to Google Forms rather than being digested by this site. This helped help things simple for us, allowing this site to be a static website while also having the form be stored on our Google Drive and able to use the [custom Google Apps Script](https://github.com/sunlightpolicy/open-data-policy-wizard) that I created to process users’ inputs.

<!-- [image of form] -->

Additionally, numerous local governments around the country have used the Open Data Policy Generator (and its predecessor resource) to help craft their open data policies. While this isn’t exactly a result of the new site — since there was a preexisting resource that did this — it’s still another piece of this that is delivering real value.

## In retrospect

I am proud of the site, and it is one of the highlights of my work at the Sunlight Foundation.

My only wish is that I had pushed a little harder on outreach to target users for testing. That said, I do think that our decisions around the release made sense given the reasons mentioned above.

## Acknowledgement

Much of the content on the site was written by other staff members over the course of years. Additionally, several other staff members contributed design and development to some of the predecessor resources.

<br><br>

**[« Back to Portfolio](/portfolio/)**
