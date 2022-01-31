## Pseudo Coding

### Front End

Single index html form with inputs for each content category in the readme
- Title
- Description
- License Selection (checkbox/radio/whatever it's called)
- Screenshot path/url
- Installation Instructions
- Usage Instructions
- Tests Included
- Collaboration
  - Checkbox for collaborators included
  - Input fields for collaborator name and github username
  - Entering into a collaborator box creates a new box below for entering more, push them all into an array 
- Contact Section

Submit puts all the info a big object and sends it in a POST to back end.

After receiving a valid response to the POST request the page hides all input fields and displays the generated readme in a new box.

Look into download requests to allow for a download button to simply grab the generated md instead of having to copy paste.

### Back End

Receives post and uses object to generate a readme using a template,
Returns the finished readme in response
Saves the generated readme as "title".md
