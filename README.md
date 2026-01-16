# DDDE-2026


https://2026.dddeurope.com/cfp/


## **TITLE**

**Releasing and recapturing informational complexity: replacing a Word template with a digital tool for Data Protection Impact Assessment.**


## **DESCRIPTION**

How do you make risk assessment something users don't describe as "hellish"?

When the Norwegian Labour and Welfare Administration (Nav) asks for, receives and uses information about its citizens, it needs to comply with laws about handling personal private information correctly. Just a few examples of these requirements: whether the state has the right to ask for the information in the first place, where and how it stores the information, who has access to the information, and whether it is only used for the stated purpose.

Nav handles a lot of personal data. It's unreasonable to expect software development teams, facilities management, benefits offices etc, to each have the expertise required to understand and document compliance with many different laws and keep up with legislative changes. Previous work at Nav has resulted in a self-assessment compliance tool where our colleagues, as individuals or teams, work through Nav's "success criteria" for compliance. These are presented (and modelled) in a highly structured way, with requirements descriptions and success criteria being owned and kept updated in the tool by subject specialist "requirements owners".

Although the compliance tool does include basic privacy legislation, colleagues must also consider whether the way they handle personal data risks compromising citizens' privacy rights. The user may conclude that they need to complete a Data Protection Impact Assessment (DPIA). This assessment involves identifying areas of potential risk, then implementing and documenting measures designed to reduce risk levels.

Until recently, DPIA was documented using a Microsoft Word template. Nav's Data Privacy Ombudsman would then review the assessment, write their comments in the same Word document and send it back to the author. Here are some of the issues with that way of doing things:

* **Because the subject domain of DPIA is more complex and cross-linked than Word could accommodate, the true domain structure just wasn't legible for many users.** Domain complexity had to be managed instead through multiple tables, repetition and manual cross-referencing. This imposed an additional, extrinsic cognitive load on top of the already substantial intrinsic cognitive load of the subject domain. Essentially, using the Word template pushed a lot of the task's inherent complexity over to the user, per [Tesler's Law](https://en.wikipedia.org/wiki/Law_of_conservation_of_complexity). Also, because of the way Word documents are shared, sent and archived within the organisation (for good reasons), it was largely impossible for authors to access other people's completed DPIAs and perhaps understand the domain better by seeing concrete examples. One of the most common words we heard from users was "uoversiktlig", which is a Norwegian word meaning roughly "impossible to get an overview of". 

* **Word is a static format that can't flex to accommodate user needs** Writing help text makes an already long document even longer, imposing additional cognitive load on all users, expert and novice. Progressive disclosure and other dynamic enhancements are not what Word was designed to do. Neither does it support dynamically inserting content from other systems: this meant a lot of manual copy/pasting for users, and the need to then maintain duplicate documentation. Word also offers limited (and obscure) functionality around reusing and linking to the same content within a single document. Filling out the DPIA template also required a lot of scrolling (another word we heard often when talking to users). These challenges all added to the extraneous cognitive load of completing a DPIA. Many of the pains were also felt by the Data Privacy Ombudsman, despite their domain expertise.

* **Word traps data.** Nav's Ombudsman has to make an annual report with qualitative and quantitative statistics about DPIAs. The Ombudsman and their team built an impressive manual workflow in OneNote to manage the Word-based system, but manual logging was time-consuming and meant less time to review DPIAs. Another user group who couldn't easily extract important information was risk owners, who had to access and read entire DPIA documents to understand the risk profile, one document at a time. 


### **(Some of) what we did** 
I would like to say a little bit about each of these, but am very open to input if you would like to see more of one thing or less of another.

* User research to understand where the old way of doing things hurt most. Our user groups include: everyday users documenting risk in their contexts, managers who then own those risks and want to understand what their risk portfolio looks like at any given time, the Data Privacy Ombudsman, and Navs own internal monitoring department. We tested frequently with users while we were in the design and build stages, and ran the new tool in private beta over the summer to get user feedback before going live. I can talk about testing, how we did it and what we found.

* Domain-mapping. One of the main challenges at the start was how to integrate the DPIA data structure with our existing compliance tool to avoid the need to duplicate common content, and instead allow content sharing and re-use where relevant. I can show some canvases where we tried to make sense of the domains, and talk a little bit about system architecture. I can also show "before" and "after" maps of how many different systems people had to use to get a DPIA done. 

* Lots of design and front-end decisions! For example, how to: visually integrate DPIA with the existing compliance tool, break down documentation into stages that made sense to users, let users create, edit, and re-use content, give users an overview of their own content, ensure incomplete content was easy to find and complete, let the Data Privacy Ombudsman view and comment on DPIAs, let users view the Ombudsman's comments, give risk owners an overview of the DPIA without too much detail, show version history and diffs … I have no shortage of Figma sketches, as well as being able to demo the tool itself.

* Automatic data aggregation and publishing. We're just starting on this now, but we hope to soon offer live performance statistics for risk owners, the wider organisation, and the Ombudsman. We should have quite a lot of dashboard data by the conference, and I can talk about what data is used by which groups, and for what. 

* As per the suggested title, one of the metaphors I'm thinking about using in the talk is carbon sequestration (!). Humans release carbon into the atmosphere through industrial processes etc. Trees and other organisms sequester carbon, reducing environmental carbon dioxide levels; when we deforest, we effectively release a bunch of CO2 back into the air. Then we ( = probably someone else not responsible for deforestation) have to find a way to sequester it again so we don't completely destroy the environment. Similarly, when we destroyed the old Word-template used for DPIA, we effectively released a lot of informational complexity that had been "captured" by the Word-template as free text with only limited structure. Our task when building the new tool was to "recapture" that complexity, but in structured ways, taking the burden off the user. The process of understanding and structuring the material demanded _way_ more time and energy than most people imagined, just as trees need water and sunlight and soil so they can do all that work. Anyway, I'm still thinking about whether it's a good metaphor, and I'd be interested to know what you think. I don't have to use it — there's plenty to show and tell without. 

* I'm attaching a couple of annotated screengrabs and a concept sketch to give an idea of what the tool looks like and just some of the design considerations that went into it. Of course when I present, I wouldn't show the annotations, but talk through it instead.

**Please add any additional notes for the organisers (links you want to share, info you want us to know,...)**

I presented at DDDE in 2024 (https://2024.dddeurope.com/program/modelling-the-law-turning-intent-into-code/) and would love to do so again if you'll have me. TI would very much have liked to come back and tell you how the work my colleague and I showed last time is now in production … but things move more slowly. The presentation I'm proposing here is loosely similar, in that it's about making better documentation tools based on user requirements, only this time it's about documentation of compliance rather than of how we implement benefits law. It's also really nice to be able to talk about a product that's actually in production and where many internal stakeholders are competing to have us prioritise their preferred features (!)

I'm very happy to discuss what you think might be the best spin on this content to fit in with the rest of the conference and any emerging themes that are coming out of other submissions. 




