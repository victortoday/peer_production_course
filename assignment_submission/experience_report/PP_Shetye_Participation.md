Akash Shetye ASS958

# Calling dibs on an issue

Once I had determined the project that I will be contributing to, I decided to look for issues that I can help fix in the project. 

## Finding a beginner task

This is very difficult for larger more popular projects as the number of available volunteers for 'beginner friendly' issues is very large. It is notoriously difficult to snag a low hanging fruit in these popular projects - this is a great sign that open source is a lot more accessible to the masses of developers. I can reflect on the pre-GitHub days of opensource, when github was not the main repository of opensource - the boundaries between opensource projects were higher, communications limited to obscure IRCs and mailing lists and interactions took place behind anonymous faceless accounts. GitHub's social angle has made it easier to consolidate these socio-technical brownie points that reflect mastery and provide a human face to the technical work, this has attracted talent that otherwise would see little upside in opensource contributions. I choose a less popular software package called react-bootstrap whi provides a react optimized package of twitter bootstrap.

## Gauging a task

After spending considerable time looking for open and do-able tasks, I came across an issue related to documenting accessibility for the collapse component who was still open [1]. This was an old issue that was probably overlooked, it also did not have the 'help wanted' or 'good first issue' tags attached to it - it had no tags attached to it. This is perhaps the reason why the issue was not taken up by any eager volunteer yet. I informed my decision by going through the conversations in its issue thread and looking at possible files that will need to be touched. I decided that I had enough skills to nail this issue.

# Being assigned the issue

Once I zeroed in on which issue I will be taking up, I left a comment in the issue thread asking if the developers were still accepting PRs. This is necessary because often projects will have duplicate issues, have abandoned the cause, things may have changed or the issue is fixed but not marked as fixed yet etc. The developers gave me a go ahead and marked the issue as taken.

The work involved in this was fairly easy, I am an experienced front-end developer and the skills helped me get a fix in. One of the two new attributes to be added to the collapse element, an attribute called 'aria-expanded' was being implicitly set by a logic not exposed to the end-user. So the question was - which setting must be honored over the other - does the implicit value take a backeast when one is explicitly defined?, as is the case usually.

# Making decisions

There are several ways this decision can pan out. Perhaps the implicit setting was a behaviour that would need to be removed now that the attributes are available for explicit setting in the component. Alternatively, the implicit setting take precedence over the explicitly specified value. I chose to defer to the council of elders (popular contributors) of the project in making a decision about this. 

# Pull request and follow up

I needed to facilitate a discussion around my fixes. I created a half-baked PR to facilitate the discussion, teh PR starts with 

> WAIT. This PR does NOT contain tests. I have a question.

I am currently waiting for community members to pitch in the discussion, once the course of action is resolved - the issue can conclude quickly. Until then I will wait for the community's participation.

References
1. React-Bootstrap Issue *[Docs] Accessibility : Should add aria-expanded and aria-controls for Collapse toggle #2825.* URL: [https://github.com/react-bootstrap/react-bootstrap/issues/2825](https://github.com/react-bootstrap/react-bootstrap/issues/2825) accessed on 25 April 2018.
