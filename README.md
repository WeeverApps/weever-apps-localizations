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

**How do I add a new language?**

Simply fork this repository (sign up for Github if you have not -- it's free), then create a new file based on your language. If you're not sure the filename to give it, just use the name of the language, we'll fix it later. Then, copy and paste the contents from one of the English language files (such as *en-US.ini*) and go through and replace each language phrase with your language.

**How do I let you know I have updates or a new language for you?**

Simply do a Pull Request. It will notify us, and we'll merge it in to our codebase.

**What if I don't want to use Github?**

Just copy one of the files from here, do the work, and open a support ticket with us with the language file attached.

**How long does it take before the new language is available in my app?**

Not long, give it a business day or so.

**Can I leave a comment in a language file?**

Yes, INI files will ignore any line starting with a semi-colon (**;**), comments may be left there. Note that this repository is public, so if you add contact information be aware it will be available for others to see.

Notes
=====

- All files should remain using UTF-8 as the encoding, in order to support non-latin alphabets.
- Keep your language strings general, not tuned to your app specifically. Your language strings will be available to all apps once deployed and will likely be corrected by someone else later. If you need some specific language in your app that is very specific to your app, please contact support.
