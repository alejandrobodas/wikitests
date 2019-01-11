# Working practices for COSP development
This document outlines the recommended working practices for COSP development. The sections below describe the workflow that any developer is expected to follow when developing changes to COSP.

## Open an issue
An issue (Github terminology) is an editable webpage that is used to provide a traceable documentation of every change: bugfix, optimization, new capability, etc. You should create an issue when you are planning a change. This issue will describe the purpose of the change. The proposed changes should be discussed with the PMC, and with the code owners of the part of COSP that is going to be modified.
It is the developers responsibility to contact the PMC at the start of this processes (the PMC will not be monitoring the issues) to ensure that proposed work is in keeping with COSP objectives and, that once developed and tested, is likely to be added to the trunk.

## Develop your change
In order to develop a change, you will need your own forked copy of the COSP repository. Once you have done that, you will create a new branch, and you will do all the code changes in your new branch. You should make regular commits to your branch to provide a history of your work that others can follow. This will help them to understand what you've done and why.

## Test your change
COSP provides you with a battery of regression tests to check that your changes don’t break the code. Test your changes regularly, not only at the end of the development process. This will help identify problems early.
This section will be expanded with examples of the testing process.

Any modification that reduces the performance and it is not protected by a logical switch (e.g. new simulator or diagnostic) will have to be strongly motivated.

## Document your change
Add meaningful comments to the source code, and modify the documentation if necessary.

## Code review
Once you are happy with the changes and documentation, and all the necessary tests have passed, you can initiate a _pull request_. If some of your changes do not pass the necessary tests, then go back and figure out why and fix the problem so that they pass the tests.

If answers change, provide a detailed explanation why the code changes modify the results. This will trigger discussion with the PMC about your changes.

The developer should assess the impact of the change and the need for a review and get agreement from the PMC. The review process is open to community members outside the PMC. If a review is considered necessary, the developer should find someone to do the review, not necessarily a PMC member.

Typically, the reviewer will suggest improvements and modifications that will lead to iterations in the modified code.  Once the reviewer is satisfied, they will approve the changes and the branch will be ready for merging.

## Merge to the master branch (trunk)
Now that your changes have been reviewed, tested, and approved, a member of the PMC will merge your code into the master branch.

## Close the issue
Once the code has been merged, the issue that documents the changes can be closed.

## Long term commitment
For major changes (e.g. new simulator), the developer will become the owner of that section. Section owners are expected to engage in a long-term commitment to help maintaining the code.
