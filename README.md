NBADrafts
=========
ID Attribute Values
-------------------
1. drafts - applied to a DIV tag, includes a list of all of the drafts present in the representation. May contain only one draft. 
2. selections - applied to  a DIV tag, includes a list of all of the draft selections present in the presentation. May contain only one selection. 
3. search - applied to a DIV tag, includes a form for query links. May contain only one form.
4. create - applied to a DIV tag, includes a form for update links. May contain only one form. 
	
Class Attribute Values 
----------------------
1. all - applied to a UL,OL tag. A list of representations. When this tag is a descendant of a  DIV.id="drafts" it may have  one or more LI.class="year" descendant elements.  When this tag is a descendant of a  DID.id="selections" it MUST have one or more SPAN.class="year" descendant element and it ma have one ormore LI.class="selection" elements.
2. details - applied to a SPAN tag. Contains a brief description of a selection. 
2. description - applied to a SPAN tag. Contains a summary description of a selection. 
3. draft-add - applied to a FORM tag. A template to add the next draft. The element MUST be set to FORM.method="post" and SHOULD contain the following descendant elements: INPUT[text].name="password".
4. draft-search - applied to a FORM tag. A template to search draft years and selections. The element MUST be set to FORM.method="get" and SHOULD contain the descendant elements: INPUT[text].name="year" and INPUT[text].name="selection".
5. multiple - applied to a UL tag. A list representation. When this tag is a descendant of a DIV.id="drafts" it may have one or more LI.class="year" descendant elements.
6. selection - applied to a LI, SPAN tag. Contains the selection of a draft. When this element is a descendant of DIV.id="selections" then it MUST contain the descendent element SPAN.class="description".
7. selections - applied to  a DIV tag, includes a list of all of the draft selections based on a query. May contain only one selection or all selections from a year.
8. selection-add - applied to a FORM tag. A template to add a draft selection. The element MUST be set to FORM.method="get" The element MUST be set to FORM.method="get" and SHOULD contain the descendant elements: INPUT[text].name="selection" and INPUT[text].name="details" and INPUT[text].name="description" and INPUT[text].name="password".
9. selection-remove - applied to a FORM tag. A template to remove a draft selection. The element MUST be set to FORM.method="get" and SHOULD contain the descendant elements: INPUT[text].name="selection" and INPUT[text].name="password".
10. single - applied to a UL tag. A list representation. When this tag is a descendant of DIV.id="drafts" it MUST have one SPAN.class="year" descendant element and may	have one DIV.class="selections" descendant element. When this tag is a decendant of DIV.id="selections" it MUST contain a LI.class="selection" element. 
11. year - applied to a LI, SPAN tag. Contains the year of a draft. When this element is a descendant of Div.id="drafts" then it MUST contain the descendent element A.rel="draft". 
	
	
Name Attibute Values
--------------------
1. description - applied to an INPUT[text] element. The team name, player name, and position of a selection. 
2. password - applied to an INPUT[text] element. The password to allow for creation and removal of selections.
3. selection - applied to an INPUT[text] element. The selection/position of the draft. The selection value to use when creating a draft position using FORM.class="selection-add". The selection value to use when removing a draft position using FORM.class="selection-remove". The search value to use when searching draft selection using FORM.class="draft-search".
4. year-end - applied to an INPUT[text] element. The year of the last desired draft. A search value to use when searching draft values using FORM.class="draft-search".
5. year-start - applied to an INPUT[text] element. The year of the first desired draft. A search value to use when searching draft values using FORM.class="draft-search".

	
Rel Attribute Values
--------------------
1. draft - applied to an A tag, a reference to a draft year. 
2. selection - applied to an A tag, a reference to a draft selection.
