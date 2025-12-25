# Personal News Agent

[![Beatles YouTube Video for "A Day in the Life"](https://img.youtube.com/vi/usNsCeOV4GM/0.jpg)](https://www.youtube.com/watch?v=usNsCeOV4GM)

This is a complete experiment in building a personal news agent that summarizes news from multiple sources, surfacing overlapping coverage, and then highlighting differences in coverage between sources.

Because it is using your browser, it can leverage your subscriptions to news sources.

The `.agent/workflows/news.md` file contains the instructions for the agent, and the workflow is roughly:

## First time setup

1. Open Antigravity User Settings
2. Go to "Browser"
3. Browser Javascript Execution Policy: Always Proceed

## Daily usage

1. Open this in Antigravity (does it work in Claude Code? IDK).
2. Run `/news` in the agent console.
3. Read the generated `news/YYYY-MM-DD.md` news summary.
4. Discuss any follow-up quesitons in the agent console.
