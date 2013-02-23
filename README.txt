
ID Attribute Values
	drafts - applied to a div tag, includes a list of all of the drafts present in the representation. May contain only one draft. 
	selections - applied to  a div tag, includes a list of all of the draft selections present in the presentation. May contain only one selection. 
	
Class Attribute Values
	all - applied to a UL,OL tag. A list of representations. When this tag is a descendant of a  DID.id="drafts" it may have  one or more LI.class="year" descendant elements.  
		When this tag is a descendant of a  DID.id="selections" it MUST have one or more SPAN.class="year" descendant element and it ma have one ormore LI.class="selection" elements.
	description - applied to a SPAN tag. Contains the description of a selection. 
	draft-add - applied to a FORM tag. A template to add the next draft. The element MUST be set to FORM.method="post" and SHOULD contain the following descendant elements: 
		INPUT[text].name="password".
	draft-search - applied to a FORM tag. A template to search draft years and selections. The element MUST be set to FORM.method="get" and SHOULD contain the descendant 
		elements: INPUT[text].name="year" & INPUT[text].name="selection".
	multiple - applied to a UL tag. A list representation. When this tag is a descendant of a DID.id="drafts" it may have one or more LI.class="year" descendant elements.
	selection - applied to a LI span tag. Contains the selection of a draft. When this element is a descendant of Div.id="selection" then it MUST contain the descendent element 
		SPAN.class="description".
	selection-add - applied to a FORM tag. A template to add a draft selection. The element MUST be set to FORM.method="get" and SHOULD contain the descendant	
		elements: INPUT[text].name="selection" & INPUT[text].name="password".
	selection-add - applied to a FORM tag. A template to remove a draft selection. The element MUST be set to FORM.method="get" and SHOULD contain the descendant	
		elements: INPUT[text].name="selection" & INPUT[text].name="description" & INPUT[text].name="password".
	single - applied to a UL tag. A list representation. When this tag is a descendant of DID.id="drafts" it MUST have one SPAN.class="year" descendant element and may
		have one DIV.class="selections" descendant element. When this tag is a decendant of DID.id="selections" it MUST contain a LI.class="selection" element. 
	year - applied to a LI, SPAN tag. Contains the year of a draft. When this element is a descendant of Div.id="drafts" then it MUST contain the descendent element A.rel="draft". 
	
	
Name Attibute Values
	description - applied to an INPUT[text] element. The team name, player name, and position of a selection. 
	password - applied to an INPUT[text] element. The password to allow for creation and removal of selections.
	selection - applied to an INPUT[text] element. The selection/position of the draft. The selection value to use when creating a draft position using 
		FORM.class="selection-add". The selection value to use when removing a draft position using FORM.class="selection-remove". The search value to use when
		searching draft selection using FORM.class="draft-search".
	year - applied to an INPUT[text] element. The year of the draft. The search value to use when searching draft values using FORM.class="draft-search".
	
	
Rel Attribute Values
	draft - applied to an A tag, a reference to a draft year. 
	selection - applied to an A tag, a reference to a draft selection.
