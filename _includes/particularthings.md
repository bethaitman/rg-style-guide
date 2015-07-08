##Error messages
Error messages are important. They're an integral part of the user experience, and users are far more annoyed by bad error messages than they are delighted by a cool UI.

* Explain, in the following order: what went wrong, why, and (if possible) how to fix it.

* Be precise. If the cause is unknown, say so.

* Be succinct. Users don't want to read an essay. They may search Google or our documentation for the error text, or quote it to the support team, so make sure it's as concise and readable as possible.

* Link to any relevant documentation. If you're not sure if there's a page describing the problem, ask a technical writer. If there isn't one and you think there should be, shout at a technical writer.

* Provide a Close button rather than OK. Having to click "OK" when an application fails makes the user feel like they're being held hostage and forced to agree to bad things.

* Don't try to be apologetic ("Sorry, your data couldn't be recovered") or funny ("Yikes! Where'd your data go?"). Keep the tone neutral and stick to the facts.

* Is the message a warning (ie something bad might happen if you continue)? Use a yellow triangle. Is it an error (ie something bad already happened)? Use a red stop icon.

* Typos add insult to injury and give a poor impression of the quality of our tools. Read the message out loud to find mistakes, and get someone else to review it.

* Where is the error message displayed? Is it a separate dialog box or in a GUI? If it's a separate dialog box, its title should typically contain the name of the application.

* Would someone who isn't a developer for this application understand the problem described?

---

##Release notes
Our release notes have been wildly inconsistent over the years. Here's our recommended format, with an example afterwards:

###Features
* Exclude words like "you can..." For example, don't write: "You can now change the number of items shown in the History dialog". Instead, write: "Change the number of items shown in the History dialog".

* List new features (and enhancements, performance improvements etc) in the release as bullet points, without full stops.

* List the features approximately in order of importance. If there's one major new feature, put it before smaller ones.

* Link to relevant documentation where appropriate (eg a page describing the feature in more detail). 

* If a feature involves changes to the UI, consider including a screenshot. This is good advertising; everyone likes a new UI.

###Fixes
* Use terms such as "now" and "no longer" to clarify that you're describing how the tool behaves in this release. Otherwise, it may sound as if you're describing the bug, not the fix. For example, don't write "Materialized views script hidden fields", as it's not clear if that's what used to happen, or what happens now. Instead, describe what the fix has changed; eg write "Materialized views no longer script hidden fields", or "Materialized views now script hidden fields", depending on what's changed.

* If the bug has a Jira reference (eg SB-5415), include it at the start of each bullet point, followed by a colon. If the same issue has multiple bug codes, include them all in the same bullet point.

* List the fixes in numerical order according to the bug code.

* If the fixes have relevant documentation, link to it.

###Known issues
* If the release introduces new issues or bugs, list them.

* If the issues have bug numbers, list them.

* Link to any relevant resources.

###Example release notes

####Features

* Upload backup copies to a SQL Backup Pro Hosted Storage account
* Manage offsite backups from the SQL Backup Pro Hosted Storage website
* View results of copying backups to hosted storage or a network location from the Activity History and Backup Properties

####Fixes

* SB-5415: When installing the server components with the /Log switch, account passwords are no longer recorded in plain text in the log
* SB-5446: The SQL Backup server components installer now checks that the user is a member of the SQL Server sysadmin role before attempting the installation

####Known issues

* SQL Backup Pro doesn't support installation on Windows Server 2012 with Failover Clustering. For more information, see Installing

---

##Usage reports
[ ] Send anonymous usage statistics and error reports to Redgate

We use these statistics to improve our tools.