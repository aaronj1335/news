---
description: Run the News Agent to gather and summarize news
---

1. For each URL in the "News Sources" section below:
    * Use the `browser_subagent` to open the URL.
    * Extract the main content and headlines.
    * Follow articles and run Javascript without requesting confirmation. Do not stop to request confirmation.
3. Summarize the collected news items:
    - Focus on the topics listed in the "Topics of Interest" section.
    - Summaries should be at least a paragraph in length.
    - The summary must link to the source material when discussing any topic.
    - Topics that appear in multiple news sources should be prioritized higher in the summary.
    - When summarizing a topic referenced in multiple sources, the must also call out differences in coverage between the sources.
4. Get the current date in `YYYY-MM-DD` format.
5. Create a new markdown file news/YYYY-MM-DD.md in this workspace.
6. Write the summary to that file, including links to the original articles.
7. Notify the user that the news summary is ready.

## News Sources

Visit the following news sites and look at the top articles:

- https://www.nytimes.com/section/todayspaper : Visit the top 20 articles
- https://www.wsj.com/ : Visit the top 20 articles
- https://www.marketplace.org/ : Visit the top 10 articles
- https://www.axios.com/ : Visit the top 10 articles

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