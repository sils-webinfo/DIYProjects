ID Attribute Values:
=====================
This design relies on four unique identifiers:

*projectHeader*
Applied to a DIV tag. The title and description of a project when the entire content is viewed.

*materials*
Applied to a DIV tag. A list of materials in the project representation. This list will contain at least one instance of the variable 'materialName' but most likely will have more than one.

*projectList*
Applied to a DIV tag. A list of all projects.

*instanceList*
Applied to a DIV tag. A list of each instance of a project that has the same project name.


Class Attribute Values
======================
This design relies on ten unique classes.

*projects*
Applied to a UL tag. A list representation.

*projectNames*
Applied to a UL tag. A list representation of projects.

*projectID*
Applied to A tag. Contains unique integer identifier for project. 

*alternateTitle*
Applied to SPAN tag. Contains alternate title of unique project.

*description*
Applied to a SPAN tag. Contains the text description of a project.

*material*
Applied to a UL tag. A list representation. 

*instructions*
Applied to a P tag. Contains the text instructions to complete a project.

*projectCreate*
Applied to a FORM tag. A link template to create a new project to the system. The element MUST be set to FORM.method="post" and SHOULD contain the following descendant elements:

*    INPUT[text]="projectName"

*projectUpdate*
Applied to a FORM tag. A link template to update content to an existing project.The element MUST be set to FORM.method="patch" and SHOULD contain the following descendant elements:

*    INPUT[text]="projectName"
*    TEXTAREA.name="description"
*    INPUT[text]="projectMaterial"

*projectSearch*
Applied to a FORM tag. A link template to search all the projects. The element MUST be set to FORM.method="get" and SHOULD contain a descendant element:

*    INPUT[text].name="nameSearch"

Name Attribute Values
=====================
This design relies on four unique names.

*projectName*
Applied to a INPUT[text] element. The name of the project.

*projectDescription*
Applied to a TEXTAREA element. The description of the project.

*projectMaterial*
Applied to a TEXTAREA element. The materials in the project.

*nameSearch*
Applied to a INPUT element. The name of the project to search for.

Rel Attribute Values
====================
This design relies on two relationships.

*project*
Applied to a A tag. A reference to a project name.

*material*
Applied to a A tag. A reference to projects made with a specific material.
