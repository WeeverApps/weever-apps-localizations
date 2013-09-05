Weever Apps Localization Strings
=========================

This repository contains the currently used files for generating language strings in Weever Apps. If you wish to add support for a new language, or update a currently supported language, just fork this repository, make your changes, and then hit 'Pull Request', and we'll take care of the rest!

FAQ
===

**How should text be formatted in these files?**

*It should follow the pattern already-present, that of 

    PHRASE_OR_WORD = "Phrase or word"
    ANOTHER_WORD   = "Another word"
  
Quotes inside the quote marks (") should be indicated using HTML entities, such as **&quote;**.

    EXAMPLE_WITH_A_QUOTE    = "&quote;Example with a quote.&quote;"
    
Would result in a string like this:

    "Example with a quote."

For other punctuations or symbols, see here for a list of codes: http://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references

**How do the language codes work? For example, what is "en-CA" mean?**

We're using ISO Language Codes (<http://www.lingoes.net/en/translator/langcode.htm>) which start with a two-letter code for the language in small letters, then a dash and two letter code for the "localization" (country/region) in capital letters.

As examples, **en-CA** referrs to **English-Canada**, and **ar-OM** referrs to **Arabic-Oman**.

**NOTE: All files should remain using UTF-8 as the encoding, in order to support non-latin alphabets.**
