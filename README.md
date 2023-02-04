# AIMARK: AI-Attribution Markdown Standard Proposal

*A draft proposal for in-line attribution of AI and human contributions within hybrid AI-assisted texts based on markdown*

### AI Disclosure & Attribution

*The majority of this document was compiled from ChatGPT replies, with light human edits.*

## Problem Statement

It is becoming increasingly difficult to identify AI-assisted (defined here as texts with both human and AI contributions) and AI-generated texts (that are majority or wholly-written by AI). And in cases of hybrid human-AI texts, to differentiate the contributions of each party.

## Why AIMARK?

AIMark is a proposed method for using custom markdown formatting to clearly differentiate between contributions made by human authors and AI in AI-assisted/generated texts. The idea is to use specific symbols, such as the percent sign `%` and forward slash `/`, to differentiate the contributions of each party to the text.

## Short Text Example:

For example, AI-generated text could be indicated with a percent sign at the beginning and end of the text, like this:

`%This text was generated by AI%`

Human-generated text could be indicated with a forward slash at the beginning and end of the text, like this:

`/This is human-generated text./`

*(Alternatively, human-generated text might not be marked at all, but AI-generated text marked.)*

Additionally, attributes such as the name of the AI model or the name of the human author can be added to the markdown by placing them in parentheses at the beginning or end of the text passage under the proposed system, like this:

```
%This text is AI generated(AI model X,3.2,OpenAI)%

%(AI model X,3.2,OpenAI)This text is AI generated%

/A human wrote this(John Doe)/ 

/(John Doe)This text is AI generated/
```

To indicate a nested human edit of an AI-generation, the format could be something like this, where `~` means strikethrough (deletion) and `^` means insertion. In the example below, we can see that the deletion and insertion happen inside of the `/`, indicating the action was taken by a human.

`%An AI-generated a big block of text and it was /~good~^bad^/%`

Under this proposed system, it would be possible to also embed global author definitions in the document, like this:

```
%% Model: AI model X, Version: 3.2, Source: OpenAI %%

// Name: John Doe //
```

By using this proposed custom markdown formatting, it will be easier for readers to understand the contributions made by both human and AI authors in AI-assisted texts in compatible display environments.

## Longer Text Blocks

In addition to the short format versions discussed earlier, AIMark also proposes a longer format version that uses square brackets `[ ]` in combination with the `/` or `%` signs to indicate AI-generated text and human-generated text respectively.

For example, a longer block of AI-generated text could be indicated with square brackets surrounding the text and percent sign at the beginning (but omitted from the end), like this:

`[%This is a longer block of AI-generated text]`

Likewise, a longer block of human-generated text could be indicated with square brackets surrounding the text and forward slash at the beginning, like this:

`[/This is a longer block of human-written text]`

This longer format version allows the markdown to indicate the author type (AI or human) without the need to close the `/` or `%` symbol, as occurs for shorter text passages when square brackets are not used.

Overall, the use of this longer format version of AIMark allows for clear and easy differentiation between AI-generated text and human-generated text, even in longer blocks of text, making it an efficient and user-friendly method for AI attribution.

## Conclusion

In conclusion, AI attribution is a valuable practice because it helps to promote trust and transparency in the use of AI-generated content. By clearly identifying and labeling AI-generated and AI-assisted content from the moment of its creation, readers and viewers can better understand the source of the information they are consuming, and make their own meaningful choices about its reliability.

## Request for Comments

We are not technical experts by any means, and welcome comments, questions, and proposed improvements to the above. Thanks for reading. 
