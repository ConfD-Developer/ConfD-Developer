# The ConfD Developer space on GitHub

We have created a public organization on GitHub to ensure we have one common place to share code for all of us working with ConfD. 

Since ConfD Developer is a public GitHub everyone can fork and read the uploaded code. By using a pull request everyone can also contribute to existing projects. 

If you want to contribute with a new project, please, read the instructions below.

## Licenses
All material in the ConfD Developer space on GitHub is under the [Apache 2.0 license](https://github.com/ConfD-Developer/ConfD-Developer/blob/master/LICENSE). The license is used to ensure a balance between open contribution and allowing you to use the software as you like to.

The license tells you what rights you have that are provided by the copyright holder. It is important that the contributor fully understands what rights they are licensing and agrees to them. Sometimes the copyright holder isn't the contributor, such as when the contributor is doing work on behalf of a company.

To ensure that the criteria in the license are met, there is a need for a Developer Certificate of Origin (DCO) sign-off on all contribution. More information about that can be found below.

## Contributing a Project on ConfD Developer GitHub
Getting Started
1.	Create an account on github.com
1.	Create your own private repository on github.com
1.	Make sure your project fulfills all the criteria listed below (under “Requirements on your project”).
1.	Send an email to the ConfD Developer librarians with a link to your repository (confd-developer-github@cisco.com).
1.	You will be added as an outside collaborator to a new repository on the [ConfD Developer GitHub](https://github.com/ConfD-Developer) and will be asked to contribute your code there.

[Read more about the implications here](https://help.github.com/enterprise/2.6/user/articles/about-repository-transfers/).

That’s it! When the move is done, your repository is now part of ConfD Developer. Keep hacking on your project, you will still have owner privileges, and as such you can decide to give others write access for example.

Users of your repository can use Issues to report bugs and suggest new features, and Pull Requests to contribute code.

When/if you do not have time to keep your project up to date (fix issues, accept pull requests, etc.) - please, say so. Write a line in the README.md, as well as an email to confd-developer-github@cisco.com - we will try to help you find a new maintainer of the code or retire it from the library if it appears abandoned for a long time.

## Expectations
When using packages from the library you can expect:

*	The code you find provided “as is” and when you use it you get to keep it. If it breaks you get to keep all the pieces.
*	If you extend a project or fix bugs, please, contribute back in the form of pull requests.

When contributing you can expect:

*	The code you contribute is made available to everyone in source form “as is”.
*	Your code might be used to: teach others about ConfD, build new products, provide a starting point for customer projects.
*	At the very minimum your contribution should have a title and a short README.md explaining what it does, see the full list of requirements below.
*	You are not required to support your contributed code, but, please, consider pull requests and try to answer questions in the project wiki.
*	Only contribute code for which you own the IPR.
*	Do not include explicit references to customers (be it customer names, network configuration / templates, or otherwise).

## Requirements on your project
Before your project can be accepted as a repository of ConfD Developer it needs to fulfill the following criteria:

### Developer Certificate of Origin
#### Signed-off
When using ConfD Developer, every commit needs to be signed-off (git commit –s) by the contributor that he or she has the right to submit it. The “-s” flag adds a line with the text 'Signed-off-by' followed by the same email address as the contributor. e.g.: 

```
My commit message

Signed-off-by Aron Aronsson <aron.aronsson@example.com>
```

It is important that your .gitconfig user.name and user.email is configured correctly.

[user]
        name = Aron Aronsson
        email = aron.aronsson@example.com

#### What is signed-off
In short you are signing off that you have the right to submit the code to ConfD Developer and that you understand that it will be public. The full text can found at [developercertificate.org](www.developercertificate.org) and also here:
```
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
1 Letterman Drive
Suite D4700
San Francisco, CA, 94129

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```
#### Signing pull requests
When creating a pull request, every commit in that pull request will be checked for DCO. If you haven’t signed all commits the checks will fail and the pull request will be denied.

Therefore, it is a good idea to sign all commits before doing the pull request.

### It should be ConfD related
Sure, it could be a cool YANG plugin too - but it should at least be relevant to ConfD application development.

### Naming
Choose a name. A good name. A catchy name, a nerdy name, a happy name - you decide. This is especially important if your contribution is a tool or a reusable library. In that case, it doesn’t even have to be descriptive. Better YxT than “YANG Extension Tool”. Don’t pick “generic-tool”, “misc-template”…

If your contribution is more of a demo or example, then a more descriptive name could be in order, perhaps even prefixed or postfixed with "demo" or "example". For example: l3-vpn-demo or example-validation-handler.

### README.md
Add a README.md. Your README.md must include:
*	Brief explanation of what your project does
*	List of dependencies (build and runtime, for example compilers, libraries, operating system)
*	Instructions on how to build the project
*	If your project contains any copies of code derived from open source, you need to explicitly list which projects.

### It must be open
The whole point of the ConfD Developer space is to share code with the ConfD ecosystem. As such, we don’t want to make it “private”. However, that means that anyone can access the ConfD Developer repositories, which requires us to approve the open access and ensure that no private information is included.

### Recommendations
*	Test cases: Add test cases and instructions on how to run them. We recommend using Lux to automate your tests? ConfD uses it!

*	Packaging: Make one repository for every standalone project. However, don’t make a lot of small repositories for things that actually belong together. It just makes the space cluttered and it will be harder to find your project.

*	Naming convention for YANG modules: For a demo or example the module name and namespace does not matter that much (you can use "example.com/..." as namespace). If your project is a re-usable piece, then consider using the URL of the project the namespace (as in: github.com/ConfD-Developer/PACKAGE-NAME/MODULE-NAME)

*	If you actually make some kind of releases, consider tagging the releases and use a “CHANGES” file or “Release Notes” document

## Link to GitHub

[ConfD-Developer](https://github.com/ConfD-Developer) 
