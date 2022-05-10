# Architecture Council Reivew

## Introduction

So, you're taking on a new piece of work. You've got some changes to make to your systems, perhaps a new one to create. You want to get these things checked out by the "Architecture Council". How do you go about that? Well, strap yourself in!

## The Architecture Council

The Architecture Council at hipages exists to help manage the architectural direction within hipages and ensure alignment to this by the teams. It meets regularly on Tuesdays at 4pm to discuss significant architectural initiatives within hipages, provide input on architecture evolution, and provide a helpdesk to those seeking advice and seeking validation of system design efforts.

## Who sits on the Architecture Council?

Current members are:
* Head of Architecture - Mo Khalil
* Architect - Joe Ruello
* VP Engineering - Jeremy Burton
* Head of Platform Engineering - Josh Vawdrey
* Head of Data - Vincent Koc
* Data Platform Technical Lead - Rukesh Kapuluru

## When Should I Present to the Architecure Council?

There's never a bad time. The Architecture Council exists to provide advice. Feel free to attend the helpdesk to ask questions, get feedback on your ideas, or generally listen in.

If you're designing a solution which has material architectural changes, then you need to seek an Architecture Council Review of the work. 

Material Changes are:
* When you're building a new product
* When you're adding a brand new feature to an existing product
* When you're creating a new system
* A change to the structure of an existing system

## The Architecture Council Review

The Architecture Council Review is your chance to present your proposed changes to the Architecture Council for endoresement. 

It's important to consider multiple options in how you implement your solution. The first thing you think of won't always be the best. There's always more than one way to accomplish an outcome, you should consider these and be especially cogniscent of the trade offs between them. 

When presenting, remember to frame the problem you're trying to solve and highlight the product/business requirements before diving into the solution and technical aspects. 

At a minimum, you should:
1. Prepare an "Architecture Council Review" doc - template is https://github.com/jeremypburton/ipr-template/blob/main/arch-council-review-template.md. 
1. Paste a link to your completed ACR doc to the #architecture-council Slack channel, and request for time at the next meeting no later than COB on the Friday before the meeting. 
1. Turn up to the meeting and talk through your proposal, answering any questions the group may have, and arrive at a formal outcome.

Additional things that will help:
* Consult with one of the architecture team before submitting and presenting, seeking feedback. This should shorten the feedback cycle and highlight any obvious challenges with your proposal,
* Invite others to present with you who might be able to provide additional support - this could include Product Managers, Engineering Managers, other Tech Leads of impacted domains, etc
* Focus on how your solution aligns to existing patterns and our architectural direction. If it's something different or establishes a new direction, provide strong reasons why existing patterns/processes/etc aren't suitable for this problem

## One more thing

Software is a living entity. We prepare designs and proposals with the best of knowledge at the time. This knowledge may be incomplete, constraints may change, or assumptions may be proven to be false in the future. That's par for the course in Software Engineering. There are (at least) two implications from this:
1. Invaribly, our deisgns will change over time. That's ok. You might get feedback that significantly alters what you've done. That's ok too. We should be able to adapt. To minimise the pain of thise, seek feedback early, seek it often.
1. By documenting our decicions like this, we snapshot our understanding at a point in time. If our understanding changes, we have a reference point that explains why we made the decision we did, and the context in which we made it (rather than assuming the current context was applicable at the time).
