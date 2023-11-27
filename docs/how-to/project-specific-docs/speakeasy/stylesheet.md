# Speakeasy style sheet

A short document covering what we know to date about the style choices you should make for Speakeasy documentation and blog posts. Very much a work in progress.

## Markup language

Speakeasy documentation and blog posts are written in [MDX](https://mdxjs.com/) (`.mdx` files). You may encounter some Markdown (`.md`) files.

MDX (Markdown with JSX) uses the same formatting syntax for basic text elements as standard Markdown. This [guide to basic Markdown syntax](https://www.markdownguide.org/basic-syntax/) shows you how to format elements like headers, bold text, italic text, lists, and links.

## Style specifics

The rules for style we highlight here are only those that deviate from the [Ritza style guide](https://styleguide.ritza.co/grammar/grammar/) or are specific to Speakeasy.

### Heading capitalization

Speakeasy documentation uses title case for titles and section headings. Use the [AP Style Book rules](https://en.wikipedia.org/wiki/Title_case#AP_Stylebook) for applying title case, or convert a heading to title case using [this tool](https://titlecaseconverter.com).

### Backticks

- In body text, place all references to code in backticks, including class names and `description` values.
- Don't use backticks in titles, headings, or subheadings because they don't render well.
- Don't put language names in backticks unless it's part of a code snippet:
    - ❌ In `go`, all types from all operations are collected into a global `AcceptHeaderEnum` type.
    - ✅ In Go, all types from all operations are collected into a global `AcceptHeaderEnum` type.

### UI element labels

Place all UI element labels like button text, menu items, tab names, section names, and page titles in bold.

### Word choice

- Prefer "create" over "generate" when referring to the Speakeasy functionality for producing SDKs.
- Refer to Speakeasy-created SDKs as "SDKs" not "client SDKs".
- Existing Speakeasy documentation uses both "auto-generate" and "autogenerate". We prefer "autogenerate".

