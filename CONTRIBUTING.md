# Contributing to the Data Stewardship Knowledgebase

Welcome to the Data Stewardship Knowledgebase!
Contributors are essential for the DSK success and usefulness, so we warmly welcome anyone who wishes to contribute.
Even tiny contributions like [opening an issue](https://github.com/MrHedmad/data-stewardship-knowledgebase/issues/new) pointing out a dead link or a type, a pull request offering new links or new chapters, or even simple a [discussion](https://github.com/MrHedmad/data-stewardship-knowledgebase/discussions) on some aspects of the DSK will be treasured.

This file lists all the tecnical, organizational and human aspects of contributing.
Thank you for taking the time to read it.

## Technical how-to
There are technical aspects that you should be familiar with before contributing via Pull Requests.
Before contributing, you should be familiar with the following technical aspects of working with Git, Github and Pull Requests:
- [About Github and Git](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git)
- You should understand what [git branches](https://docs.github.com/en/get-started/quickstart/github-glossary#branch) are and how they work.
  - You might find [this guide from Atalassian](https://www.atlassian.com/git/tutorials/using-branches) helpful.
- [About repositories](https://docs.github.com/en/get-started/quickstart/create-a-repo).
- Pages are written in Markdown and are interpreted by MdBook to webpages.
  You can read more about Markdown [here](https://www.markdownguide.org/getting-started/),
  and Github's Markdown guide [here](https://guides.github.com/features/mastering-markdown/).
  You can read more about MdBook [here](https://rust-lang.github.io/mdBook/).
- You should understand how the pull request process works.
  You can read more about it [here](https://docs.github.com/en/get-started/quickstart/github-flow).

You are also required to:
- Install [Git](https://git-scm.com/) on your local machine and configure it.
  - You can read more about git configuration [here](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup).
  - There is also this [GitHub guide](https://docs.github.com/en/get-started/quickstart/set-up-git).
- Have a GitHub account. You can read how to create one [here](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account).

You might find [this comprehensive guide for git and github](https://wpmudev.com/blog/the-non-developers-guide-to-git-and-github/) useful.

When you are ready, read [Contributing to a project](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) for a guide on how to fork the repository, add your changes, and propose them for inclusion.
A lot of information on how to contribute to a community, as well as specifically on Github, is collected in [The Turing Way chapter on Collaboration](https://book.the-turing-way.org/collaboration/collaboration).

Here are some additional resources that you may find helpful:
- [GitHub Documentation](https://docs.github.com/)
- [Open Source Guides](https://opensource.guide/)

The rest of this guide is for specific information on the structure, rationale and *modus operandi* of the Data Stewardship Knowledgebase.

## Legal aspects of contributing
When contributing, you agree that all your contribution will be licensed under the license specified in the [LICENSE](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/LICENSE) file.
You will be asked to sign off the [Developer Certificate of Origin](https://developercertificate.org/) when you contribute.
Feel free to contact any person on the core maintainer team (detailed at the bottom of the page) for further clarification on this step.
In simple (and non-legally binding) English, you essentially acknowledge that you hold the copyright for your contribution and that it, as well as the name that you used to submit that contribution, will be licensed under the open-source license detailed in the license file of the project in perpetuity.

## Code of Conduct
When you engage with the community, you also agree to follow the [Code of Conduct](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/CODE_OF_CONDUCT.md).

## License
By contributing to this project, you agree that your contributions will be licensed under the [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) license as specified in the [LICENSE](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/LICENSE) file in the root directory of this repository.

## Recognition of Contributors

The DSK has a clear code of conduct and policy regarding the recognition of its contributors.
You can read this code of conduct [here](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/CODE_OF_CONDUCT.md).
Practically, all contributors are listed in the [CONTRIBUTORS](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/CONTRIBUTORS.md) file, aided by the help of the [All-contributors bot](https://allcontributors.org/).

---

# Structure of the Data Stewardship Knowledgebase

The DSK aims to be a handbook of useful resources for both current Data Stewards handling data and future Data Stewards-to-be which are just approaching the subject.
To this end, it has a few main goals:
- Define what data stewardship is, and provide insight on what meaningful data stewardship should look like in different contexts, with particular emphasis in the context of public research.
- Aggregate in an orderly way the resources found scattered on the internet, as data management can be a diffuse topic touching many aspects in many different contexts;
- Integrate information from other websites with additional context and, if needed, create new resources to fill in gaps from publicly available knowledge.
- Define lists of best practices and methods, as well as providing ways to find and define such methods, in a wide array of contexts;
- Provide practical guides and how-tos to deal with common or recurring problems when dealing with data stewardship and management in different contexts.
- Promote principles of meaningful data stewardship in many research contexts, and provide teaching material useful to promote such principles to a wide audience by Data Stewards and other people interested to do so.
- Promote the critical evaluation of the philosophy of science and the method of doing science of research groups and institutions through the collection of useful resources and teaching materials.

The DSK is structured in four broad categories of interest: Open Science, Computer Science Toolbox, Policy and Legal Issues and Stewarding the Data Lifetime.
They are described below, so that you may be aware of the overarching structure of the DSK.

## Open Science
The profession of Data Steward, and the concept of meaningful, useful data stewardship for the benefit of the community is the culmination of years of Open Science philosophy.
This section aims to explore the aspects of Open Science, in particular in the context of data management.
It covers topics such as:
- What Open Science is;
- Why is Open Science the right direction for researchers and research institutions to take;
- What could go wrong if Open Science is implemented badly;
- What do Data Stewards do in the context of Open Science;
- How to efficiently teach Open Science concepts to others;
- Why data and data stewardship matters so much for Open Science;
- Why a third party (like a researcher) might be interested in implementing Open Science and Data Stewardship policies;

## Computer Science Toolbox
In the modern day, data is almost always manipulated digitally in some form.
Even physical objects might be listed in a digital index, or scanned and digitalized altogether.
For this reason, a Data Steward has to have some computer science knowlege and a toolbox of digital hammers and wrenches which are useful when dealing with digital data.
This section covers topics such as:
- What digital data is;
- How digital data is encoded, transmitted and shared with others;
- What formats are available to save data in;
- What is metadata and in which formats are available to represent it;
- What data infrastructures are and how to manage them (as potential administrators);
- Technologies to manipulate, reshape, fuse and split data;
- Determination of costs related to data management (e.g. storage and computing power);
- Knowledge of relevant tools that can be used to obtain, reshape, reuse, manipulate and share data throughout a research project.

## Policy and Legal issues
The administration of data, especially personal data, may be subject (or should be subjected) to laws.
This section aims to aggregate such concepts and make a data steward both aware of them and capable of dealing with them.
It covers topics such as:
- National and International privacy laws regarding personal data;
- Legal issues when reusing other’s code and data;
- Ethical concerns of releasing, reusing and otherwise manipulating data;
- Determining the ethical and legal risks related to handling specific types of data;
- How to give recognition when reusing a piece of data produced by others;
- Creation of effective Open Science policies and plans of action for groups and organizations;
- Fulfilling Open Science/Data Stewardship requirements for funding bodies that require them (i.e. DMPs);
- The soft skills required for effective management and administration of an organization interested in implementing data stewardship practices;

## Stewarding the data lifetime
The most expansive and eterogeneous section, "Stewarding the data lifetime" deals with the philosophical, pratical and technical aspects of data stewardship, from the planning of data collection, to the manipulation of fresh data, to its potential deletion or archival, etc...
This section is heavily context-specific: ideas that might apply to data in the context of biological science might not be relevant to Architectural studies, and vice-versa.
This section covers many topics, and some examples include:
- How to plan data collection, even at large scales and with many data collection partners;
- Determining when, where and how to store newly created data;
- Defining and measuring data quality for specific data types in specific contexts;
- Designing and implementing data curation procedures, from collection to archival;
- Solving the discard problem and defining methods and formats of long to very-long term preservation of archive data;
- Determining the best methods of reusing published data to limit useless expenditures, with particular regards to ascertaining data quality and usefulness for the purpose.

---

# Ways to contribute
This section lists all the main ways that you can contribute to the DSK, and how to best approach doing so.

## Contributing with Feedback
We value your feedback! If you have any suggestions, questions, or concerns, please don't hesitate to reach out.
Here are the ways you can contribute with feedback:
- If you find something wrong about the DSK, or would like to propose changes, [open an issue in the repository](https://github.com/MrHedmad/data-stewardship-knowledgebase/issues/new) and detail what you found to be wrong, including a link to the incriminated resource or page, if possible.
- Start [a discussion](https://github.com/MrHedmad/data-stewardship-knowledgebase/discussions/new/choose) or [join the Discord Server](https://discord.com/invite/Ww3rWRsEDz) to simply chat about the DSK.
- Contact the maintainers directly. You can find a list of maintainers at the bottom of this guide.

## Contributing links
The DSK is mainly composed of links to other resources.
When you think you have found a good resource to add to the DSK, open a pull request with your changes.
Keep in mind that:
- The link should be included in the most relevant section, or sections, of the DSK.
- The link should not be affected by [link rot](https://en.wikipedia.org/wiki/Link_rot). For methods of avoiding link rot, please peruse the Wikipedia article for the definition of link rot (linked before). An useful service to save existing pages before linking them in the DSK is using [the Wayback Machine](http://web.archive.org/).
- The source of the information should be reliable. In short, a reliable source is one generally recognized to be accurate, truthful and persistently available in time. It can be useful to peruse [Wikipedia's article on reliable sources](https://en.wikipedia.org/wiki/Wikipedia:Reliable_sources).
- A link should be tagged following the [emoji key](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/src/emoji_key.md) based on the link's content. The anatomy of the link should look like this:
  ```
  This is a :hammer: :closed_lock_with_key: [link](https://example.com) to a tool that requires a login.
  ```
  Note how the emojis are immediately before the link proper and spaced out with a single space between them and between the last emoji and the link.

(Work in progrss...)
