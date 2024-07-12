# The Data Stewardship Knowledgebase Style Guide

To ensure consistency across the repository, the DSK follows a specific style guide, detailed below.

## Folder structure
The DSK is generated with [mdbook](https://rust-lang.github.io/mdBook/), so it follows its basic structure in the `src` folder.
The DSK is divided into several broad topics, each with its own folder.
Within each topic, there are subcategories and individual files for specific resources.

Each top-level topic folder should contain a `README.md` file that serves as an introduction to the topic, and should be indexed in the `SUMMARY.md` file.
This file should provide an overview of the topic and link to relevant subcategories or resources.
Each such `README.md` file contains the main content of the topic, and generally it contains the majority of the information and links related to that topic.
Please include a table of content for easier navigation.

Each top-category `README.md` file can be accompanied by any number of additional files, which can be used to provide more detailed information or to organize resources in a more granular way.
Each of these files should be linked in the main `README.md` file in the "Specific Resources" section AND in the `SUMMARY.md` file.
These additional notes may be collections of links, prose about a topic, or any other relevant information.

## File formats
All files are written in markdown to be parsed by [mdbook](https://rust-lang.github.io/mdBook/).

## Link description
When adding links to the DSK, please tag them following the [Emoji Key](emoji_key.md).
New emojis may be added parsimoniously if none of the old ones are useful for a resource.
This helps to quickly identify the type of resource being linked and provides a visual cue for users.
Link tags should be placed at the beginning of the link proper, with a space between them and the start of the link.

Each link may be followed by a longer description in prose, describing the linked content.
When writing such a description, be terse but complete.
Try to answer the following questions, from the point of view of the reader:
- Why should I read this resource?
- What is inside of this resource that I will find interesting or useful?
- Should I have previous knowledge in order to understand this resource?

## Prose
When writing prose, please use clear and concise language.
Avoid jargon or overly technical terms unless they are necessary for understanding the content. If you are unsure about the clarity of your writing, consider asking for feedback from other contributors. Provide links to external resources where appropriate to help readers learn more about a topic
