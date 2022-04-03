# Release notes for versions 2.x

**NOTE**
Even already the follow up of "dita13.lc.extra-interactions" already exists, "eu.xstructuring.dita.lce" v3p0,  
we decided to also make a new version for "dita13.lc.extra-interactions" because most vendors and clients still use "dita13.lc.extra-interactions".

It is not defined yet if the changes will be moved to the 3.0 version or if the 3.0 version will be deleted. Most of the important changes are already in 2.6.


Version 2.6
- new attributes for answers
  - answerlength - for gaps, t-shirt sizing
  - answerlines - for open questions, integer
  - answerformat - mainly for gaps, values: text, math, decimal, integer, date
  - answernumbercorrect - for e.g. hotspot if all hotspot are correct but only a certain amount must be chosen
  - outputorder - if shuffle is not wanted and the order must be a certain
- new attribute: questiontype - to define the sort question, at the moment only "opinion"
- new attribute: placeholder - for text which must be overwritten by the end-user
- new question element: lceInlineOrder - new question in which words or fragements within a sentence can be ordered; add to the inline interactions
- new element: lceMarginal - special element for content e.g. hyperlinks which must stand the marginal in a print product; in a digital product it should be mouse over or something like that. 
- changed content model of lcInteraction, now the div element is allowed as child of lcInteraction; this is done by adding div to the group lceperforminteraction-d-lcInteractionBase2

Version 2.5
- new elements: lceCalculation, lceFraction, with children lceNumerator and lceDenominator), lceMathSign and lceMathPh. The lceCalculation should only be used in the lceTextEntry.
- new elements: lceHottextMeaning and lceRef. In the lceHottextMeaning should be used to define the meaning of a hottext. From the lceHottextOption you can use the lceRef element to link the right meaning.
- new elements: lceBox - should be used for special content which has a title and mostley is displayed as box

Version 2.3 / 2.4
- new interaction: lceGraphicAssociate - interaction where you can reate hotspots and set relation between hotspots (drawing lines)
- new element lceExplanation: based on div, available in undbounded choice group with lcAsset2; should be used to explain the content/context of a question/answer
- new attribute contentclass, based on base; should be used for the semantic meaning of an element instead of outputclass

Version 2.2.1
- Changed content model of lcePerformQuestion.content: add lcOpenAnswer2

Version 2.2
- new interactions: lceChainMatching - matching items from more than two bukkets

Version 2.1
- new interaction: GraphicTextEntry