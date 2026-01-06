---
description: Run the News Agent to gather and summarize news
---

// turbo-all

1. Make a directory `news/YYYY-MM-DD`, where `YYYY-MM-DD` is the current date.
    * If this directory is already there, assume that you are restarting the task. Do not re-do work you've already done, re-create any files, or change things.

2. The "News Sources" section below has a configuration for several different news sources. Each item in this top level list is a "news source configuration". For each item in the "News Sources" section:
    * Make a directory in `news/YYYY-MM-DD` with whatever name is listed in the news sources "Sub-directory for this news source".
        * So for example, for a Wall Street Journal news source, on 2026-01-01, you would have the directory `news/2026-01-01/wsj`.
    * Use the `browser_subagent` to open the "Starting page" URL.
    * ONLY VISIT NEWS SOURCES LISTED IN THE "News Sources" SECTION. Do not infer which news source to use.
    * Make a list of the top articles.
        * Limit the length of the list to the "Number of articles to visit" listed in the news source's configuration.
        * It is ok if the articles you found on the starting page for the news source are from previous days.
        * Do not include op-eds or opinion articles.
        * Write this list in an `articles.md` Markdown file in the news source's sub-directory. Include the starting page URL. So for example, for a Wall Street Journal news source, on 2026-01-01, you would have the file `news/2026-01-01/wsj/articles.md`.

    * For each link in the articles.md file for the news source, use the `browser_subagent` to navigate to the article and read the contents.
        * Summarize the article in a Markdown file in the news source's sub-directory.
        * Article summaries should generally be 3-5 paragraphs long
        * Summaries must take care to include relevant facts and statistics.
        * The name of the Markdown file should be like a URL "slug" with underscores. So for example, for an article from a Wall Street Journal news source, on 2026-01-01, you may have the file `news/2026-01-01/wsj/a_look_back_at_the_economy_of_2025.md`.
        * Make sure the name of the markdown file isn't more than 100-200 characters though.

3. Read all of the Markdown files in the `news/YYYY-MM-DD/` directory (and sub-directories) and create a summary:
    * Only use the directory from step 1. So if the date is 2026-01-01, only create the summary from Markdown files within the `news/2026-01-01` directory.
    * Focus on the topics listed in the "Topics of Interest" section.
    * Summaries should be at least a paragraph in length.
    * The summary must link to the source material when discussing any topic. The links should be text links, not numbers, (i.e. `[5.1](https://nytimes.com/abc-def-ghi)` is bad, instead have informative link text like `[NY Times article on ABC DEF GHI](https://nytimes.com/abc-def-ghi)`)
    * Topics that appear in multiple news sources should be prioritized higher in the summary order.
    * When summarizing a topic referenced in multiple sources, the must also call out differences in coverage between the sources.
    * Write this summary to a `summary.md` file. So for example, on 2026-01-01, you would write to the file `news/2026-01-01/summary.md`.

## News Sources

Visit the following news sources and look at the top articles:

1. NY Times
    * Starting page URL: https://www.nytimes.com/section/todayspaper
    * Sub-directory for this news source: `nyt`
    * Number of articles to visit: 4
2. Wall Street Journal
    * Starting page URL: https://www.wsj.com/
    * Sub-directory for this news source: `wsj`
    * Number of articles to visit: 4
3. Marketplace
    * Starting page URL: https://www.marketplace.org/
    * Sub-directory for this news source: `marketplace`
    * Number of articles to visit: 2
4. Marketplace
    * Starting page URL: https://www.axios.com/
    * Sub-directory for this news source: `axios`
    * Number of articles to visit: 2

## Topics of Interest

Focus on the following topics:

- Economics, finance, and business
- Technology and innovation
- China
- US sanctions or economic policies applied to other countries
- Events local to Austin Texas or Indiana
- Open source software
- Google
- AI
- Javascript, Python, and Android
