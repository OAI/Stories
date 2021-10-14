# Content Archive

## Brief

The Stories repository serves a number of purposes with one being the capture, curation and publication of content on OpenAPI: articles, podcasts, videos, etc.

Clearly holding this kind of material in text files has limited value and will need to be render in something readable and searchable for normal human beings. However, its important to start capturing this collateral so this directory serves as a holding bay ready for publication.

The approach is bound to evolve over time. Expect refactoring :grimacing:.

## Current Approach

> **THIS IS SUB-OPTIMAL AND WILL BE REFACTORED BUT ITS CONVENIENT FOR WHERE DEVELOPMENT IS RIGHT NOW!**

Steps:

* Create a directory with the search date.
* Touch the content files.

Script:

```bash
content_directory=src/content/$(date +%Y"-"%m"-"%d)
mkdir $content_directory && touch $content_directory/articles.yaml $content_directory/podcasts.yaml $content_directory/videos.yaml
```

## Evolution

Ideas:

* Content analysis to workout automatically what the keywords are (there are plenty of commerical tools available for this, at a cost...).