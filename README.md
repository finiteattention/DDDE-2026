# DDDE-2026


https://2026.dddeurope.com/cfp/


## **TITLE**

**Making a complex domain legible to users: replacing a Word template with a digital tool for Data Protection Impact Assessment.**


## **DESCRIPTION**

How do you make risk assessment a process users don't describe as "hellish"?

The Norwegian Labour and Welfare Administration (Nav) handles a lot of information about citizens. Nav must comply with several detailed sets of regulations, such as GDPR. It must also document that compliance on a large scale.

It's unreasonable to expect software development teams, facilities management, benefits offices etc, to each have the expertise required to understand and document compliance with many different laws, and to keep up with legislative changes. Previous work at Nav has resulted in a self-assessment compliance tool to help individuals or teams work through Nav's "success criteria" for compliance. These are presented (and modelled) in a highly structured way, with requirements descriptions and success criteria being owned and kept updated in the tool by subject specialist "requirements owners".

Where there is potential risk to citizens' privacy rights, teams may also need to complete a Data Protection Impact Assessment (DPIA). Until recently, DPIA in Nav was documented, reviewed and signed off on using a Microsoft Word template. Word as a format was challenging for users (many of whom are not familiar with DPIA or privacy legislation), for Nav's data privacy ombudsman who reviews DPIAs and returns them with feedback, and for risk owners in the organisation who need an up to date overview of their risk portfolio.

This talk will outline how Nav went from using Word for DPIA, to building integrated support for DPIA into the existing compliance tool. The talk will demo the tool itself (in production since September 2025) and touch on:

* What happens to the user experience, and domain knowledge, when a documentation tool (Word) is too simple for the domain being documented.

* Cognitive load as a lens for thinking about user needs in documentation tools.

* Using domain mapping and user feedback to decide how to integrate new functionality into an existing tool.

* Designing for users to create and re-use their own content while retaining an overview of what is used where.

* Practical design considerations when allowing users to complete regular compliance and DPIA documentation side by side. 

* Designing to make it as hard as possible to produce a "bad" DPIA.

* Integrating functionality for three distinct user groups, each with different requirements, into the same tool.

* Harnessing user pains to prioritise feature development

* Designing with data in mind from the beginning. 

department. We tested frequently with users while we were in the design and build stages, and ran the new tool in private beta over the summer to get user feedback before going live. I can talk about testing, how we did it and what we found.

* Domain-mapping. One of the main challenges at the start was how to integrate the DPIA data structure with our existing compliance tool to avoid the need to duplicate common content, and instead allow content sharing and re-use where relevant. I can show some canvases where we tried to make sense of the domains, and talk a little bit about system architecture. I can also show "before" and "after" maps of how many different systems people had to use to get a DPIA done. 

* Lots of design and front-end decisions! For example, how to: visually integrate DPIA with the existing compliance tool, break down documentation into stages that made sense to users, let users create, edit, and re-use content, give users an overview of their own content, ensure incomplete content was easy to find and complete, let the Data Privacy Ombudsman view and comment on DPIAs, let users view the Ombudsman's comments, give risk owners an overview of the DPIA without too much detail, show version history and diffs … I have no shortage of Figma sketches, as well as being able to demo the tool itself.

* Automatic data aggregation and publishing. We're just starting on this now, but we hope to soon offer live performance statistics for risk owners, the wider organisation, and the Ombudsman. We should have quite a lot of dashboard data by the conference, and I can talk about what data is used by which groups, and for what. 

* As per the suggested title, one of the metaphors I'm thinking about using in the talk is carbon sequestration (!). Humans release carbon into the atmosphere through industrial processes etc. Trees and other organisms sequester carbon, reducing environmental carbon dioxide levels; when we deforest, we effectively release a bunch of CO2 back into the air. Then we ( = probably someone else not responsible for deforestation) have to find a way to sequester it again so we don't completely destroy the environment. Similarly, when we destroyed the old Word-template used for DPIA, we effectively released a lot of informational complexity that had been "captured" by the Word-template as free text with only limited structure. Our task when building the new tool was to "recapture" that complexity, but in structured ways, taking the burden off the user. The process of understanding and structuring the material demanded _way_ more time and energy than most people imagined, just as trees need water and sunlight and soil so they can do all that work. Anyway, I'm still thinking about whether it's a good metaphor, and I'd be interested to know what you think. I don't have to use it — there's plenty to show and tell without. 

* I'm attaching a couple of annotated screengrabs and a concept sketch to give an idea of what the tool looks like and just some of the design considerations that went into it. Of course when I present, I wouldn't show the annotations, but talk through it instead.

**Please add any additional notes for the organisers (links you want to share, info you want us to know,...)**

I presented at DDDE in 2024 (https://2024.dddeurope.com/program/modelling-the-law-turning-intent-into-code/) and would love to do so again if you'll have me. TI would very much have liked to come back and tell you how the work my colleague and I showed last time is now in production … but things move more slowly. The presentation I'm proposing here is loosely similar, in that it's about making better documentation tools based on user requirements, only this time it's about documentation of compliance rather than of how we implement benefits law. It's also really nice to be able to talk about a product that's actually in production and where many internal stakeholders are competing to have us prioritise their preferred features (!)

I'm very happy to discuss what you think might be the best spin on this content to fit in with the rest of the conference and any emerging themes that are coming out of other submissions. 




