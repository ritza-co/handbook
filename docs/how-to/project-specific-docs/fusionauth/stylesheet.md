# FusionAuth style sheet

FusionAuth has comprehensive [documentation guidelines](https://github.com/FusionAuth/fusionauth-site/blob/master/DocsDevREADME.md) that you can familiarize yourself with. This style sheet is where we track the information that we find most relevant to the content we produce for FusionAuth.

## Markup languages

FusionAuth documentation is written in AsciiDoc (`*.adoc`). Take a look at the [AsciiDoc Syntax Quick Reference](https://docs.asciidoctor.org/asciidoc/latest/syntax-quick-reference/) for formatting tips.

FusionAuth blog posts are formatted in Markdown (`*.md`). Here's a guide to [basic Markdown syntax](https://www.markdownguide.org/basic-syntax/).

## Style specifics

The rules for style we highlight here are only those that deviate from the [Ritza style guide](https://styleguide.ritza.co/grammar/grammar/) or are specific to FusionAuth.

### Heading capitalization

* FusionAuth documentation uses [title case](https://styleguide.ritza.co/grammar/grammar/#capitalization) for titles and section headings. You can use this [title case converter](https://titlecase.com) to apply title case rules to your headers correctly.
* FusionAuth blog posts use sentence case for titles and section headings.

### Personal pronouns

* Use second person not first person plural ("you" not "we").

### Code snippets

* Don't use a colon before a code snippet. End the introductory sentence with a period.
* Use title case for code captions.

### Classes

* Use classes instead of backticks in the following cases:
    * Referencing a field in a form or JSON API doc: `[field]` for example, `[field]#Issuer#`.
    * Referencing a UI element or button: `[uielement]` for example, "Click the `[uielement]#Ok#` button".

### Links

* Links should be fully qualified and never include a slash at the end: `link:/docs/v1/tech/apis/users`.

### FusionAuth preferred formatting

* Id (not ID, referring to a unique identifier)
* curl (not Curl or cURL)
* pre-configured (not preconfigured)

Find more FusionAuth formatting preferences in [this list](https://github.com/FusionAuth/fusionauth-site/blob/master/DocsDevREADME.md#proper-names-and-other-verbiage).
