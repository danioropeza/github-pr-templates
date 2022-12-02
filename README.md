# Educate developers through GitHub Pull Requests Templates

One of the most critical roles we play as developers is to clearly communicate with our team.

As a developer, I want the team members who will review my code to understand what I'm trying to achieve with my work. And as a code reviewer, I want the developer to explain their changes and let me know how I can test their code.

GitHub allows us to create [Pull Request Templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository). This feature is very helpful because we can communicate all of our ideas in one place. We can encourage contributors to communicate more effectively with their teams by noting what’s new and changed.

Also, using pull request templates is a way of educating developers because with the information we remember the developers to do some verifications before creating the pull requests.

### What does this repository have?

In this repository you can find an example of a Pull Request template. [Click here](https://github.com/danioropeza/github-pull-request-templates/blob/develop/.github/pull_request_template.md) to see our example.

### Explanation of the Pull Request Template example

![image](https://user-images.githubusercontent.com/33135078/205185353-fa6efb3d-666a-498e-91c3-50ea3016db51.png)

1 ) Planning tool ticket number, it can be JIRA/Trello/GitLab and so forth.

2 ) Type of pull request. Many times Pull Requests add changes to the UI, backend, unit test or automation. Here we describe in which sections you make the changes.

3 ) .

4 ) This section is to mention some important things to the Code Reviewer before starting to review the Pull Requests. Information is added that cannot be clarified with the previous points.

5 ) As the  name says, they are relevant screenshots. It can be screenshots of the Unit Tests working well, of the production build working well, visual changes in the UI, etc.

6 ) This section is to help the developer to verify some points before sending the Pull Requests. The following points remind the developer:

&emsp; 6.1) not to merge code without first doing a rebase with the integration branch.

&emsp; 6.2) if the Pull Request meets the ticket acceptance criteria.

&emsp; 6.3) if it can be used as valuable documentation for the future. In other words, when we go back in time to see the history, could it be useful to see the Pull Request?

&emsp; 6.4) verify that new or existing inputs have data validations.

&emsp; 6.5) the possibility of failure scenarios, think about them and think about how to solve them if they appear.

&emsp; 6.6) .

&emsp; 6.7) verify that everything is working well with Swagger.

&emsp; 6.8) verify that all the new visible texts for the user have their localization keys.

&emsp; 6.9) verify that the changes in the User Interface are responsive with different screen dimensions.

&emsp; 6.10) verify that QA is aware of my changes.

&emsp; 6.11) .

&emsp; 6.12) verify that the changes in the database do not affect the existing data in production.

&emsp; 6.13) verify that our implementation has Unit Tests.

&emsp; 6.14) verify that the Unit Tests and e2e are working fine and not broken.

&emsp; 6.15) A pull request with many changes is more difficult to review. That is why it is better that they are short and easy to read.

&emsp; 6.16) verify that the changes I'm adding don't have other foreign changes, and only do one thing.

&emsp; 6.17) many times we send pull requests without verifying that we can refactor the code even more. Have I really reviewed the changes I'm adding?

7 ) Reminder to specify what was not ticked, and the reasons.

This article is also in Medium [Educate developers through GitHub Pull Requests Templates](https://medium.com/@danioropezasoria/educate-developers-through-github-pull-requests-templates-41b7c64287f7).
