## Code coverage is a lie

### Introduction

I believe in test-based development (TDD) as it improves code quality and  [responsibility](https://paritosh.hashnode.dev/the-motivation-for-writing-tests-first). But it also allows bad practices to seep into the organization e.g. code coverage. My eyes roll when anyone mentions that "our code coverage is 95% or our code coverage is a feature" and I almost die inside. I have also seen this as a feature of the product (where is laughing well). I would try to provide reasons why I am saying so:

### Code is a liability 

Producing more code does not equate to results. If you have high code coverage, it means there are lots of tests that have been written. It will drive the maintenance cost of the tests itself very higher. 

Very soon all tests will be converted into legacy and no one will maintain or review it. You might see this in legacy codebases. By the time you realize, Tests are blocker major blockers in releasing features. 

### No more safety net

I have seen very often that codebases have been modified but no related Tests have been modified. It means Tests were written to satisfy the code coverage but not to catch bugs or alarm developers if something is wrong. 

It was supposed to provide a safety net for developers when they are introducing new functionalities. This is one of the reasons we write tests. So if your tests are not broken or modified after writing a new feature or fixing a bug, Some tests are useless and removed at once.

### Very less confidence in releasing features 

If the codebase's code coverage is high and still developer fear releasing new software, You might want to review tests. Also if a new release is breaking on production under these circumstances is a very good indicator of this issue. 

### Summary

Code coverage is bad metrics that should not be part of the team's success. Time is a precious resource in software development, Use it wisely. 

