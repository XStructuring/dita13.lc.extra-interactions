# Release notes for versions 2.x

**NOTE**
Even already the follow up of "dita13.lc.extra-interactions" already exists, "eu.xstructuring.dita.lce" v3p0,  
we decided to also make a new version for "dita13.lc.extra-interactions" because most vendors and clients still use "dita13.lc.extra-interactions".

It is not defined yet if the changes will be moved to the 3.0 version or if the 3.0 version will be deleted. Most of the important changes are already in 2.6.

Version 2.7
- new shell XSD voor lceMap; now a map with all lce attributes can be used
- new attributes for list, box and table layout
  - oltype: defines the style of the ol, values are: decimal, upper-latin, lower-latin, upper-roman, lower-roman and lower-greek
  - ultype: defines the stype for the symbol used, values are: bullet, dash, circle, blank, square, checkbox and arrow
  - olstart: defines with which number should be started if different from 1
  - olhierarchicalsep: defines the seperator which should be used for nested ol
  - boxwidth: defines the relative width of a box
  - boxheight: defines the relative height of a box
  - rowheight: defines the height of a row
  - linestyle: defines how the line/border of a box, table, colom, row or entry should look like.
  - conerradius: defines if an how round the coners of a box should be.
- new attributes for using colors
  - color: type xs:string, can be used to define the color of a text (using the ph element)
  - background: type xs:string, can be used to define the background color of text (using the ph element), box, table, col, row and entry.
- new attribute position: can be used to define the position in the print layout

Version 2.6.1 and 2.6.2
- Bugfixes

Version 2.6
- new attributes for answers
  - answerlength - for gaps, t-shirt sizing
  - answerlines - for open questions, integer
  - answerformat - mainly for gaps, values: text, math, decimal, integer, date
  - answernumbercorrect - for e.g. hotspot if all hotspot are correct but only a certain amount must be chosen
  - outputorder - if shuffle is not wanted and the order must be a certain
- new attribute: questiontype - to define the sort question, at the moment only "opinion"
- add value "inexact" to attribut answertype; should be used for text entry questions when the answer can variate a bit
- new attribute: placeholder - for text which must be overwritten by the end-user, usually used for text entry questions
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