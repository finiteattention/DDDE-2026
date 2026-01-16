# DDDE-2026


https://2026.dddeurope.com/cfp/


## **TITLE**

**Releasing and recapturing informational complexity: building a digital tool for Data Protection Impact Assessment.**


## **DESCRIPTION**

How do you make risk assessment something users don't describe as "hellish"?

When the Norwegian Labour and Welfare Administration (Nav) asks for, receives and uses information about its citizens, we need to comply with the laws about handling personal private information correctly. Just a few examples of these requirements: whether the state has the right to ask for that information in the first place, where and how it stores the information, who has access to the information, and whether the information is only used for the stated purpose.

Nav processes a lot of personal data. It's unreasonable to expect software development teams, facilities management, benefits offices etc, to each have the expertise required to understand and document compliance with many different laws, and to keep up with changes in legislation. Previous work at Nav has resulted in a self-assessment compliance tool where our colleagues, as individuals or teams, work through the various requirements and Nav's "success criteria" for compliance. These are presented (and modelled) in a highly structured way, with requirements descriptions and success criteria being owned and kept updated in the tool by subject specialist "requirements owners".

Although the compliance tool does include basic privacy legislation, users must also consider whether the way they process personal data risks compromising citizens' privacy rights. The user may conclude that they need to complete a Data Protection Impact Assessment (DPIA). This assessment involves identifying areas of potential risk, then implementing and documenting measures designed to reduce risk levels.

Previously, DPIA was documented using a Microsoft Word template. Nav's Data Privacy Ombudsman would then review the assessment, write their comments in the same Word document and send it back to the author. Here are some of the issues with that way of doing things:

* **Because the subject domain of DPIA is more complex and cross-linked than Word could accommodate, the true domain structure just wasn't legible for many users.** This complexity instead had to be managed through multiple tables, repetition and manual cross-referencing. This imposed an additional, extrinsic cognitive load on top of the already complex intrinsic cognitive load of the subject domain. Essentially, the Word template pushed a lot of the task's inherent complexity over to the user, per [Tesler's Law](https://en.wikipedia.org/wiki/Law_of_conservation_of_complexity). Also, because of the way Word documents are shared, sent and archived within the organisation (for good reasons), it was largely impossible for authors to access other people's completed DPIAs and perhaps understand the domain better by seeing concrete examples.

* **Word is a static format that can't flex to accommodate user needs** Writing help text makes an already long document even longer, imposing additional cognitive load on all users, expert and novice. Progressive disclosure and other dynamic enhancements are not what Word was designed to do. Neither does it support dynamically inserting content from other systems: this meant a lot of manual copy/pasting for users, and the need to maintain duplicate documentation. Word also offers limited (and obscure for all but power-users) functionality around reusing and linking to the same content within a single document. Filling out the DPIA template required a tremendous amount of scrolling (and "scrolling" was one of the most commonly used words when we talked to users). These challenges all added to the extraneous cognitive load. 

* **Word traps data.** Nav's Ombudsman has to make an annual report with qualitative and quantitative statistics about DPIAs. The Ombudsman and their team built an impressive manual workflow in OneNote, but manual logging was time-consuming and meant less time to review DPIAs.


### **(Some of) what we did:**

* User research to understand where the old way of doing things hurt most. Our user groups include: everyday users documenting risk in their contexts, managers who then own those risks and want to understand what their risk portfolio looks like at any given time, the Data Privacy Ombudsman, and Navs own internal monitoring department. The most commonly used word when talking to users was "uoversiktlig", which is a Norwegian word meaning roughly "impossible to get an overview of". We tested frequently with users while we were in the design and build stages, and ran the new tool in private beta over the summer to get user feedback before going live. I can talk a little bit about the first, brave team to get their DPIA all the way through the review and signoff process while we were still finishing building the tool.

* Domain-mapping. One of the main challenges at the start was how to integrate the DPIA data structure with our existing compliance tool to avoid the need to duplicate common content, and instead allow content sharing and re-use where relevant. I can show some canvases where we tried to make sense of the domains, and talk a little bit about system architecture. I can also show "before" and "after" maps of how many different systems people had to use to get a DPIA done. 

* Lots of design and front-end decisions! For example, how to: visually integrate DPIA with the existing compliance tool, break down documentation into stages that made sense to users, let users create, edit, and re-use content, give users an overview of their own content, ensure incomplete content was easy to find and complete, let the Data Privacy Ombudsman view and comment on DPIAs, let users view the Ombudsman's comments, show version history and diffs … I have no shortage of Figma sketches as well as being able to demo the tool itself.

* Automatic data aggregation and publishing. We're just starting on this now, but we hope to soon offer live performance statistics for risk owners, the wider organisation, and the Ombudsman.

* As per the suggested title, one of the metaphors I'm thinking about using in the talk is carbon sequestration (!). Humans release carbon into the atmosphere through industrial processes etc. Trees and other organisms sequester carbon, reducing environmental carbon dioxide levels; when we deforest, we effectively release a bunch of CO2 back into the air. Similarly, when we destroyed the old Word-template used for DPIA, we effectively released a lot of informational complexity that had been "captured" by the Word-template as free text with only limited structure. Our task when building the new tool was to "recapture" that complexity, but in structured ways, taking the burden off the user. The process of understanding and structuring the material demanded _way_ more time and energy that most people imagined, just as trees need water and sunlight and soil so they can do all that work. Anyway, I'm still thinking about whether it's a good metaphor, and I'd be interested to know what you think. I don't have to use it — there's plenty to show and tell without. 


**Please add any additional notes for the organisers (links you want to share, info you want us to know,...)**

I presented at DDDE in 2024 (https://2024.dddeurope.com/program/modelling-the-law-turning-intent-into-code/) and would love to do so again if you'll have me. Last time I and my colleague presented the proof of concept of a tool designed to model the law so we could map the relationship between primary legislation and how it is actually implemented in code. I'd love to be able to say that my proposal this time is the same work that's now in production, but unfortunately our organisation has other ideas … so instead, I'd like to talk about the work I've been doing since then. It's a similar concept: the organisation has to to document how it complies with legislation, only this time it's compliance in the sense of data privacy laws rather than benefits law.




