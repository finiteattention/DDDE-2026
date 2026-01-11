# DDDE-2026


https://2026.dddeurope.com/cfp/


**TITLE**

**Releasing and capturing informational complexity: A case study in building a digital tool for Data Protection Impact Assessment.**


**DESCRIPTION**
~~For Norwegian citizens to get welfare benefits and other help that they are entitled to, The Norwegian state needs information about them.~~ 

When the Norwegian state asks for, receives and uses information about its citizens, it needs to comply with the laws about handling personal private information correctly. Just a few examples: whether the state has the right to ask for that information in the first place, where and how it stores the information, who has access to the information, and whether the information is only used for the stated purposes. 

Norway has about 5.6 million citizens, which is small by European standards, but in GDPR terminology, the various organs of the Norwegian state are data controllers on a large scale. 

The Norwegian Labour and Welfare Administration (Nav), which pays out benefits and helps get people into work, will touch most citizens' lives at some point. We process a lot of personal data, and we are responsible for ensuring compliance with data protection legislation, and for documenting that compliance.

Where there is additional risk that citizens' data privacy rights may be compromised, further work is needed. This is the Data Protection Impact Assessment (DPIA), where the data controller (the appropriate state organ) identifies areas of high potential risk, describe them, and take measures to reduce the level of risk.

Conducting a DPIA is important, but so is documenting it. Nav needs to be able to say 

Nav has previously developed a digital tool for documenting general compliance across a range of legislative requirements, including data privacy. However, until recently, it did not have a tool for documenting DPIA. This talk is about how we went from documenting DPIA in Word-documents sent by email [CAN WE SAY THIS???] to 








**Please add any additional notes for the organisers (links you want to share, info you want us to know,...)**

Hi there :) I presented at DDDE in 2024 (https://2024.dddeurope.com/program/modelling-the-law-turning-intent-into-code/) and would love to do so again if you'll have me. Last time I and my colleague presented the proof of concept of a tool designed to model the law so we could map the relationship between primary legislation and how it is actually implemented in code. I'd love to be able to say that my proposal this time is the same work that's now in production, but unfortunately our organisation has other ideas … so instead, I'd like to talk about the work I've been doing since then. It's a similar concept: the organisation has to to document how it complies with legislation, only this time it's compliance in the sense of data privacy laws rather than benefits law.

One of the metaphors I'm thinking about using in this talk is carbon sequestration (!). Humans release carbon into the atmosphere through industrial processes etc. Trees and other organisms sequester carbon, reducing environmental carbon dioxide levels; when we deforest, we effectively release a bunch of CO2 back into the air. Similarly, when we destroyed the old Word-template used for DPIA, we effectively released a lot of informational complexity that had been "captured" by the Word-template as free text with very limited structure. Our task when building the new tool was to "recapture" that complexity, but in structured ways. This demanded _way_ more energy that most people imagined (I think they expected we would just remake the Word template in HTML), just as trees need water and sunlight so they can do their thing. Anyway, I'm still thinking about whether it's a good metaphor, and I'd be interested to know what you think. It's also kind of adjacent to Tesler's law about the inherent, irreducible complexity of a thing being work that either the UI takes care of (if we designers do a good job), or else the user has to.



