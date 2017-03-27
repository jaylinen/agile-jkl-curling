# Markdown style guide

This file is written in valid [Markdown syntax](http://daringfireball.net/projects/markdown/basics).

All training material should be written in Markdown.

Text paragraphs, and pretty much all other elements should be separated with an empty line. Many markdown renderers
fail if you e.g. have a title right before a list without an empty line in between.

For readability, keep the maximum line length shorter than 120 characters.

## Titles

Precede titles with one or more hashes (atx-style). Do not use dash underlining (setex-style). Use at most three
levels of headers. Surround titles with an empty line.

<!-- markdownlint-disable MD025 -->

# Example of top level title

## Second-level title

### Third-level title

<!-- markdownlint-enable MD025 -->

## Unordered lists

- Use dashes in unordered lists.
- Do not use asterisks or plus signs.
- Surround a list with empty lines.
  - You can also have nested items (but remember that less is more).

## Links and images

You can use [hyperlinks](http://daringfireball.net/projects/markdown/basics).

To make images, prefix link syntax with an exclamation mark ![Short text to explain the image](https://github.com/gofore/aws-training/raw/b782150624c2793fbbe2ce281ebb336c99e01479/images/aws_list_of_services.png)

TBD: Should local links be relative or absolute?

## Emphasis

Use single asterisks to *make italic text*.

Use double asterisks to **make bold text**.

## Horizontal rulers

Horizontal rules are only used to separated slides from each other.

Use double hyphen to separate a vertical subslide in reveal.js.

--

Use triple hyphen to separate a horizontal slide in reveal.js.

---

TBD: Should we use 2-dimensional slide layout?
