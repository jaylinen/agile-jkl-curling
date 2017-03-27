# Contribution guidelines

- Each module should be independent, and should not directly depend on the contents of other modules. Some modules may
  form a module series as they cover a large topic. But even in this case, the material should not directly refer to
  the previous module, e.g. "continue where we last left", "as mentioned in the previous module". A person who knows
  the basics of a topic, should be able to smoothly skip the basic module and complete the advanced module on its own.
- All material should be shareable with the participants, and thus should be considered public. Please note this with
  customer project warstories.
- Each module should consist of a single Markdown-file. This file can then be presented as a JavaScript presentation
  or rendered into PDF/HTML.
- Follow the [Markdown](/doc/markdown_styleguide.md) guidelines of the project.
- The baseline for the presentations is the old [aws-training](https://github.com/gofore/aws-training/tree/master/docs).
- All material should be written in English. This includes documentation and commit messages.
- All exercises should work on all major operating systems. There should be minimal tooling involved.
- Use Unix line endings.
