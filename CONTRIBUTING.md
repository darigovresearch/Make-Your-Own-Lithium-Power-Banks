# Contributing
To make this project extensible as far into the future as possible we are following certain rules which will also make it possible to programmatically pull the data.

Pull requests, corrections, translations & fixes are welcome. Any contributions must be submitted under the same license that the original piece of work (see below). Take a look at any open issues or submit new ones if there is something that needs to be fixed or added.

Watch our video on how to contribute to open source for a complete overview -> [https://www.youtube.com/watch?v=UWA4wyacY2A](https://www.youtube.com/watch?v=UWA4wyacY2A)

## Folder and Filename conventions
Every language should be saved in a folder called `lang-code` for example `[fr]` for French. In each folder you save
- .tex source file,
- .pdf output file
- and an Images folder for images that have any text in them that require translation

**Each source .tex file has three parts to it:**
1. en
2. _make_your_own_lithium_power_banks
3. .tex

**Explanation**
1. is the language code for the given language,
2. is literally `Make Your Own Lithium Power Banks` translated into the language that the pdf is in but lowercased & with underscores instead of spaces,
3. is the extension file to make it readable by the correct text editors & other computer programs (here it is a tex file)

### Translating for other languages
Translations in all languages are welcome. Send a pull request or open an issue any time of day or night.

**Please prepend the tag `[lang-code]` to your issues and pull requests.** For example, `[fr]` for French. This will help everyone pick out things they care about.

We're happy for any contribution in any form, but if you're making more than one major change (i.e. translations for two different languages) it would be super cool of you to make a separate pull request for each one so that someone can review them more effectively and/or individually.

## Requesting a new language
You can request a language via an issue request with the following title `[lang-code]: Language Request` and body text:

```
*New language* has been requested, having the following in *New language* to build out the folder structure would be helpful to begin the translation of each chapter

1. Preface
2. Introduction
3. Basic concepts
4. Risks and dangers of lithium-ion batteries
5. What are lithium-ion battery cells?
6. Collecting 18650 cells
7. Building a USB power bank
8. Building a bigger battery pack
9. Lithium battery chemistries, applications and form factors
10. Resources
11. Appendix

Other terms
1. Make Your Own Lithium Power Banks
```

Supplying the new language translation of all the chapter titles means that we can create the corresponding folder structure & to make it easier for you to just translate the content. In the future we hope to have code to auto generate the file structure for you but this is currently work in progress.

## File structure
The preface is very important as if it is not visible the user will not know where they can find updates, corrections and improvements to the PDF.

Please work from the first to the last section for consistency when translating into a new language as it also means that some can learn using your translation before having all the sections.

## Steps for submitting a new translation
The general process for porting existing translations to make a new language is the following:
1. Make a fork of the latest version of the repository
2. Download it to your local computer
3. Copy the source files which contains definitions in a language that you speak
4. Rename the filename translating the correct words if required
5. Translate the front of each card along with it's explanation
6. Check your work (it is much easier to make corrections before many people have downloaded your translated PDF than after)
7. Generate the .pdf file with the correct filename using your preferred LaTeX distribution
8. Make a pull request

## Building the sphinx experiment
As stated in the readme there is a [sphinx-based](https://www.sphinx-doc.org/en/master/) version [at this URL](https://darigovresearch.github.io/Make-Your-Own-Lithium-Power-Banks/) which may end up being easier to convert to offline pdfs & a more interactive site. After cloning the repository if you wish to edit or make improvements to it, you need to edit the relevant files in the `docs_source` folder and when you want to build it, you run the following command from the root folder of the repository. The output will then be able to be opened locally from the `docs` folder.

```
sphinx-build docs_source/source docs
```

## Style Guidelines
- Do make sure punctuation is consistent across translations
    - This includes but is not limited to spaces, brackets, quotation marks, question marks, asterisks, exclamation points, ellipses etc.
- Do follow the naming conventions for file and folder names above
- Refrain from adding additional context to a translation as it may not be relevant
- Do not use any online translation tools or dictionaries to help with the translation
    - We want this project to be a human-led endeavour as people tend to understand the context of translation better than computer generated tools
