# Information about the translationAcademy Manuals

### Explanation of the content file layout

The files containing the text for each article are in the `content` directory of the repository. The content of the files are in a hybrid YAML/markdown format, beginning with a YAML header followed by the body of the article in markdown.

YAML is a markup language that is compact and easy to read. The YAML header bounded on the top and bottom by `---`. Each line within the header is a key-value pair, with the key and the value separated by a colon. Because the key is used by the publishing process, __it should never be translated or changed.__ Some of the values can be translated, and those are enumerated below in the instructions for translating.

Following the YAML header is the body of the article, which uses a format called "markdown." If you aren't familiar with markdown, you may find [this tutorial](http://www.markdowntutorial.com/) helpful. Also, this README file, the one you are reading now, is written in markdown.


### Before you get started translating

* DO NOT RENAME ANY FILES. The name of the file is the same as the slug and is used to link the file to other files.

* If you do any translation work, be sure to put your name in the `CONTRIBUTORS.md` file.

* The `LICENSE.md` file does not need to be translated.


### Instructions for translating translationAcademy

__The instructions for translating `meta.yaml` (metadata) and `toc.yaml` (table of contents) are included in the header of those files.__

The first step is to __fork this repository.__ When you do this, change the name of the repository to start with your language code rather than
`en`.

All of the content pages for this translationAcademy (tA) module are located in the `content` directory. The following list is refering to these files.

* In the YAML header, you are free to translate the values following the `title`, `question` and `credits` keys. __DO NOT TRANSLATE THE KEYS__.
None of the other values should be translated. They contain slugs that are used to identify this article and to link it to other articles.

* Translating hyperlinks: Hyperlinks (links to other articles or to other pages on the internet) follow this pattern,

```
[text to display](http://www.example.com)
```

You can translate the "text to display" inside the square brackets but not the web address that follows inside the parentheses.

You are free to add additional pages. In order for the new page to be included when tA is published, all of the following conditions need to be satisfied:

  1. It must be in the `content` directory, no sub-directories allowed.

  2. The file extension must be `.md`.

  3. The file must be included in the table of contents, `toc.yaml`.

  4. The value of the slug in the YAML header and the file name (without the extension) must be the same.

  5. The slug must be unique, and not used in any of the other tA repositories. This is a requirement so that it is possible to create unambiguous links to articles in other tA manuals.
