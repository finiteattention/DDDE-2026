# DDDE-2026


https://2026.dddeurope.com/cfp/


**TITLE**

**Releasing and capturing informational complexity: A case study in building a digital tool for Data Protection Impact Assessment.**


**DESCRIPTION**

How do you make risk assessment something users don't describe as "hellish"?

When the Norwegian Labour and Welfare Administration (Nav) asks for, receives and uses information about its citizens, we need to comply with the laws about handling personal private information correctly. Just a few examples of these requirements: whether the state has the right to ask for that information in the first place, where and how it stores the information, who has access to the information, and whether the information is only used for the stated purposes.

We process a lot of personal data, and we are responsible for ensuring compliance with data protection legislation, and for documenting that compliance. It's unreasonable to expect software development teams, facilities management, benefits offices etc, to each have the expertise required to understand and document compliance with all the different requirements and updates in legislation. Previous work at Nav has resulted in a self-assessment compliance tool where our colleagues, as individuals or teams, work through the various requirements and success criteria in a highly structured way, documenting as they go. Requirements descriptions are owned and kept updated in the tool by subject specialist "requirements owners".

Although the compliance tool also covers privacy requirements, users must consider whether the data processing they are documenting also risks impinging on citizens' data privacy rights. The user may conclude that they need to complete a Data Protection Impact Assessment (DPIA). The assessment involves identifying areas of potential risk and documenting them, then implementing and documenting measures designed to reduce risk levels.

Previously, documentation of DPIA was done in a Word-template. Our Data Privacy ombudsman would then review the assessment, write their comments in the same Word document and send it back to the user. This way of doing things presented several challenges. Here are some:

**DPIA is a challenging subject with high intrinsic cognitive load.** 

* Many of our users do not have a high level of subject knowledge about data privacy, but are still required to make a thoughtful and detailed analysis of risk and consequences. Word didn't support contextual help and other types of enhancements one could use to assist those struggling with an unfamiliar domain. 

* Because the subject domain is more complex and cross-linked than Word could accommodate, the DPIA domain structure wasn't legitible for many users. 
*
* Struggling through a form that required repetition and referring back to other sections didn't give users the overview they needed. 

* Word could not connect different parts of the document for re-use or two-way cross-linking, or keep a running tally of anything you were doing.
*  It couldn't Instead, users were mired down in repeating themselves or referring to other places in the table. Essentially, the Word template pushed a lot of the complexity over to the user, per [Tesler's Law](https://en.wikipedia.org/wiki/Law_of_conservation_of_complexity). 

*
* And because of the way Word-documents are sent and archived, it was also effectively impossible to access other people's completed DPIAs to read them, and perhaps understand better what was required.

**Word imposed additional extrinsic cognitive load:** 

* Word doesn't support dynamically pulling in content from the same document or from other tools, or reusable content with a single source. 


* The content you need to produce in a DPIA overlaps partially, but not wholly, with regular privacy compliance documentation. Users completing a DPIA typically copy-pasted a lot of content over to Word from our compliance tool and were frustrated at having to produce and maintain duplicate documentation.


* The cognitive challenge 

For example, users of the DPIA template had to manually copy and paste some of their documentation from the compliance tool.


* Extraneous cognitive load. Word doesn't support help text and other enhancements, so filling out  a big table in Word is not a good format if you are struggling with an unfamiliar subject domain (many of our users aren't, or don't have access to, data privacy specialists).  Scrolling up and down in a long document when you are writing one section that refers to another section only adds to the cognitive load.

* Nobody truly _liked_ working in Word, even the Personal Privacy Ombudsman who knew it inside out.
* 
* You can't connect a Word document to any other systems beyond adding links. 
* Word doesn't allow aggregation of data about compliance across the organisation, which led to a lot of manual reporting.

Nav has previously developed a digital tool for documenting general compliance across a range of legislative requirements, including data privacy. However, until recently, it did not have a tool for documenting DPIA. This talk is about how we went from documenting DPIA in Word-documents sent by email [CAN WE SAY THIS???] to 

**Labour-intensive**

* Manual reporting


**(Some of) what we did:**

* User research to understand where the old way of doing things hurt most. Our user groups include: everyday users documenting risk in their contexts, leadership who then own those risks, the Data Privacy Ombudsman, and different parts of the organisation who need data about risk and compliance. The most commonly used word was "uoversiktlig", which is a Norwegian word meaning roughly "impossible to get an overview of". Other favourites were "scrolling" and TODO. We tested frequently with users while we were in the design and build stages, and ran the new tool in private beta over the summer to get user feedback before going live.

* Domain-mapping. One of the main challenges at the start was how to integrate the DPIA data structure with our existing compliance tool to avoid the need to duplicate common content, and instead allow content sharing and re-use where relevant. I can show some canvases where we tried to make sense of the domains, and talk a little bit about system architecture. I can also show "before" and "after" mapping of how many different systems people had to use to get a DPIA done. 


* Lots of design and front-end decisions! How to: visually integrate DPIA with the existing compliance tool, break down documentation into stages that make sense to users, let users create, edit, and re-use content, give users an overview of their own content, ensure incomplate content is easy to find and complete, let the Data Privacy Ombudsman view and comment on DPIAs, how to let users view the Ombudsman's comments, how to show version history and diffs … I have no shortage of Figma sketches as well as being able to demo the tool itself.

* 


* Start publishing data about DPIA and compliance for the organisation. We're just starting on this now, but
* One of the benefits should be much less manual reporting for the Data Privacy Ombudsman.



**Please add any additional notes for the organisers (links you want to share, info you want us to know,...)**

Hi there. I presented at DDDE in 2024 (https://2024.dddeurope.com/program/modelling-the-law-turning-intent-into-code/) and would love to do so again if you'll have me. Last time I and my colleague presented the proof of concept of a tool designed to model the law so we could map the relationship between primary legislation and how it is actually implemented in code. I'd love to be able to say that my proposal this time is the same work that's now in production, but unfortunately our organisation has other ideas … so instead, I'd like to talk about the work I've been doing since then. It's a similar concept: the organisation has to to document how it complies with legislation, only this time it's compliance in the sense of data privacy laws rather than benefits law.

One of the metaphors I'm thinking about using in this talk is carbon sequestration (!). Humans release carbon into the atmosphere through industrial processes etc. Trees and other organisms sequester carbon, reducing environmental carbon dioxide levels; when we deforest, we effectively release a bunch of CO2 back into the air. Similarly, when we destroyed the old Word-template used for DPIA, we effectively released a lot of informational complexity that had been "captured" by the Word-template as free text with very limited structure, leaving users to manage that complexity. Our task when building the new tool was to "recapture" that complexity, but in structured ways, taking the burden off the user. This demanded _way_ more energy that most people imagined (I think some expected we would just remake the Word template in HTML), just as trees need water and sunlight so they can do all that work. Anyway, I'm still thinking about whether it's a good metaphor, and I'd be interested to know what you think. It's also kind of adjacent to Tesler's law about the inherent, irreducible complexity of a thing being work that either the UI takes care of (if we designers do a good job), or else the user has to.



