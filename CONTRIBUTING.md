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

### Code of Conduct
When you engage with the community, you also agree to follow the [Code of Conduct](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/CODE_OF_CONDUCT.md).

### License
By contributing to this project, you agree that your contributions will be licensed under the [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) license as specified in the [LICENSE](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/LICENSE) file in the root directory of this repository.

## Recognition of Contributors

The DSK has a clear code of conduct and policy regarding the recognition of its contributors.
You can read this code of conduct [here](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/CODE_OF_CONDUCT.md).
Practically, all contributors are listed in the [CONTRIBUTORS](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/src/CONTRIBUTORS.md) file, aided by the help of the [All-contributors bot](https://allcontributors.org/).

---

# Structure of the DSK
Each section of the DSK has an Index page with the introduction to the topic and links to other sections.
These sections are in `src/topics`.

These pages include introductory or propedeutic resources.
Other pages in the section refer to specific topics or macro-areas of discussion.

---

# Ways to contribute
This section lists all the main ways that you can contribute to the DSK, and how to best approach doing so.

## Contributing with ideas and feedback
We value your feedback! If you have any suggestions, questions, or concerns, please don't hesitate to reach out.
Here are the ways you can contribute with feedback:
- If you find something wrong about the DSK, or would like to propose changes, [open an issue in the repository](https://github.com/MrHedmad/data-stewardship-knowledgebase/issues/new) and detail what you found to be wrong, including a link to the incriminated resource or page, if possible.
- Start [a discussion](https://github.com/MrHedmad/data-stewardship-knowledgebase/discussions/new/choose) or [join the Discord Server](https://discord.com/invite/Ww3rWRsEDz) to simply chat about the DSK.
- Contact the maintainers directly. You can find a list of maintainers in the [CONTRIBUTORS](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/src/CONTRIBUTORS.md) file.

## Contributing links
The DSK is mainly composed of links to other resources.
When you think you have found a good resource to add to the DSK, open a pull request with your changes.
Keep in mind that:
- The link should be included in the most relevant section, or sections, of the DSK. The introduction of the DSK has a description on all of its sections.
- The link should not be affected by [link rot](https://en.wikipedia.org/wiki/Link_rot). For methods of avoiding link rot, please peruse the Wikipedia article for the definition of link rot (linked before). An useful service to save existing pages before linking them in the DSK is using [the Wayback Machine](http://web.archive.org/).
- The source of the information should be reliable. In short, a reliable source is one generally recognized to be accurate, truthful and persistently available in time. It can be useful to peruse [Wikipedia's article on reliable sources](https://en.wikipedia.org/wiki/Wikipedia:Reliable_sources).
- A link should be tagged following the [emoji key](https://github.com/MrHedmad/data-stewardship-knowledgebase/blob/main/src/emoji_key.md) based on the link's content. The anatomy of the link should look like this:
  ```
  This is a :hammer: :closed_lock_with_key: [link](https://example.com) to a tool that requires a login.
  ```
  Note how the emojis are immediately before the link proper and spaced out with a single space between them and between the last emoji and the link.
- Include with your link a short description on what resource this link entails, and why one would want to access and consume the resource. Try to answer the questions:
  - Is this interesting for an existing Data Steward? Does it answer some question, solve some problem or provide insight?
  - Is this useful for people who want to become Data Stewards? Is it complete, informative and easy to digest?
  - Is this resource a practical manual, or operative example? Would it be widely applicable?
  If you replied with "yes" to any of these, the link probably has a place in the DSK.

All proposed resources will be evaluated by the community and the maintainers for adherance to the above principles, and will be included or rejected at the maintainer's discretion.
Feel free to propose again a rejected link if the resource changes or you think it can now be included in the DSK.

Some exclusion criteria for links are:
- They do not adhere to the Community Guidelines;
- They are opinion pieces far from the general consensus on a topic;
- The resource is prone to change, is still in development or is incomplete;
- The resource is paywalled, and requires a very high entry fee.

## Contributing text
Some topics are not well covered in existing resources.
While external resources are priviledged, the DSK may host textual information internally if such information is not well covered online.

If you think there is such a topic which could be covered in such a way, feel free to create a new page, or section in an existing resource, and propose it for inclusion.

Consider these aspects when creating such a resource:
- Cite external sources while you write. The DSK is not a place for opinion pieces or personal anecdotes. Be sure that the entry you are working on is backed up by data, facts, external resources or has community support. Footnotes are a good place for references.
- Be concise and to the point. Do not user overly technical language, when not necessary. While this point applies to all internal DSK resources, there is no hard limit on the lenght of such items.
- Consider that the DSK has learning as one of its aims. Therefore, try to include introductory or propedeutic material at the start of the section.
- Consider linking to further learning material at the end of the piece.
