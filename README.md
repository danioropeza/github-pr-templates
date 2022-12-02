# Enhance changes communication through GitHub Pull Requests Templates

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

3 ) verify when you expect this fix to be deployed. This should help the Reviewer determine if the branch you’re targeting is the right one, and to consider other implications of going on that release.

4 ) This section is to mention some important things to the Code Reviewer before starting to review the Pull Requests. Information is added that cannot be clarified with the previous points.

5 ) As the name says, they are relevant screenshots. It can be screenshots of the Unit Tests working well, of the production build working well, visual changes in the UI, etc. Something you can explain with pictures. Sometimes a picture is worth a thousand words.

6 ) This section is to help the developer to verify some points before sending the Pull Requests. The following points remind the developer:

&emsp; 6.1) not to merge code without first doing a rebase with the integration branch. This is a common mistake in developers, they merge the code without rebasing, we can avoid this with this simple reminder.

&emsp; 6.2) if the Pull Request meets the ticket acceptance criteria. Double check that it complies with everything specified in the ticket so you don’t have to add new changes later.

&emsp; 6.3) if it can be used as valuable documentation for the future. In other words, when we go back in time to see the history, could it be useful to see the Pull Request?

&emsp; 6.4) verify that new or existing inputs have data validations. This applies to both front-end and back-end.

&emsp; 6.5) verify that the asynchronous calls have their corresponding catches, and that we do not miss an error that kills the application. Think in the possibility of failure scenarios and think about how to solve them if they appear.

&emsp; 6.6) verify that we are writing sufficient and useful logs. Remember that the logs are for developers, not end users. The logs have to help the developer to troubleshoot. You have to ask yourself… Are the logs enough to interpret the context when an error occurs?

&emsp; “Typing File Not Found” doesn’t help at all. We need to know what file you were looking for, so we can try to do something.

&emsp; 6.7) verify that everything is working well with Swagger.

&emsp; 6.8) verify that all the new visible texts for the user have their localization keys. Remember that a word can have few characters in one language and many in another language. Verify that the user interface does not break with very long and short texts.

&emsp; 6.9) verify that the changes in the User Interface are responsive with different screen dimensions.

&emsp; 6.10) verify that QA is aware of my changes. Let’s not forget that for a product to be of quality, it must be tested many times. Therefore, it is important to test our changes before merging the code.

&emsp; 6.11) Generally, there should be documentation on how to build the product. If you download it from scratch and try to compile to start working, ideally there should be a few steps. If that documentation becomes obsolete, it is serious. Because a developer wouldn’t know how to start, and would have to figure it out.

&emsp; 6.12) verify that the changes in the database do not affect the existing data in production. Remember that the most valuable thing in the company is the user data, you must take care of them like gold and avoid any losses or inconsistencies.

&emsp; 6.13) verify that our implementation has Unit Tests.

&emsp; 6.14) double check that the Unit Tests and e2e are working fine and not broken.

&emsp; 6.15) A pull request with many changes is more difficult to review. That is why it is better that they are short and easy to read.

&emsp; 6.16) verify that the changes I’m adding don’t have other foreign changes, and only do one thing. It should only do what the ticket says, if you want to add something, it is much better to create another ticket for that.

&emsp; 6.17) many times we send pull requests without verifying that we can refactor the code even more. Have I really reviewed the changes I’m adding?

7 ) Reminder to specify what was not marked and if I can clearly explain the reasons why it was not marked.

This article is also in Medium [Educate developers through GitHub Pull Requests Templates](https://medium.com/@danioropezasoria/educate-developers-through-github-pull-requests-templates-41b7c64287f7).
