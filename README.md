# Application
Test Application

<p>This test application was built using Zend Framework 2.</p>

<h3>Notes</h3>
For the purpose of this test, ZF2's default routing has not been utilised as it requires modifications to nginx and/or Apache config. With that in mind, once you've installed, the homepage directory is located at:

[wherever/you/uploaded.dev]/gov.uk/public/application/index

<h3>Setting up</h3>
<p>Download the zipped file and extract to wherever on your web server you intend to test from. Once uploaded, Go to "[wherever/you/uploaded.dev]/gov.uk/public/application/index". You should see the home page.

<h3>Testing</h3>
<p>There are five controller actions, each reading and/or writing to an SQLite database included in the repository (for portability). These are:</p>
<ul>
<li>Index action: the home page. No tests required.</li>
<li>Add action: add a new application. Each field should be mandatory. If any fields are empty, the form will not submit and validation messages will be displayed to the user. If all fields are completed, on submit a new entry in the database will be created and the user will be redirected back to the homepage.</li>
<li>Edit action: editing an existing application. Each field should be mandatory. If any fields are empty, the form will not submit and validation messages will be displayed to the user. If all fields are completed, on submit the corresponding entry in the database will be updated and the user will be redirected to the view page for that application.</li>
<li>View action: view an existing application/ No tests required.</li>
<li>Delete action: delete an application. If a valid application ID is provided, the corresponding entry in the database will be deleted and the user will be redirected back to the homepage</li>
</ul>
