# UK AI prices, availability and local LLM fit: open data from aiagents.org.uk

Four small datasets behind the trackers on [aiagents.org.uk](https://aiagents.org.uk/), a UK guide to AI agents and private, local AI. Each row is checked against the vendor's own page, and each file shows the date it was checked.

| File | What it holds | Rows | Source page |
|---|---|---|---|
| `data/uk-ai-prices.csv` / `.json` | UK monthly prices for AI assistants, coding tools, automation, meeting and image tools: plan, price, billing, VAT, vendor source and date checked | 32 | [UK AI price tracker](https://aiagents.org.uk/uk-ai-price-tracker/) |
| `data/uk-ai-cheapest-routes.csv` / `.json` | The cheapest paid route to each main assistant in the UK, and what to avoid | 6 | [UK AI price tracker](https://aiagents.org.uk/uk-ai-price-tracker/) |
| `data/uk-ai-agent-availability.csv` / `.json` | Which AI agents work in the UK, which are limited and which are not here yet, with the UK catch | 25 | [AI agents UK availability](https://aiagents.org.uk/ai-agents-uk-availability/) |
| `data/local-llm-mac-fit.csv` / `.json` | Which local models fit a Mac with 8 to 128 GB of memory: Ollama tag, download size, fit, licence | 40 | [Best local LLM for Mac](https://aiagents.org.uk/best-local-llm-mac/) |

Last updated: 21 November 2026.

## How the data is made

- **Prices:** read from each vendor's UK pricing page or the UK App Store. Prices in dollars are shown in dollars with an approximate pound figure; VAT is recorded as the vendor states it ("Included", "Excluded" or "Not stated").
- **Availability:** read from each maker's help pages, country lists and launch notes. "Limited" means it works in the UK with a named restriction.
- **Local LLM fit:** download sizes are what Ollama gives a Mac, read from its registry. Ollama now downloads Apple's MLX build of a model on a Mac where one exists, so some sizes differ from those on Ollama's website. Fit uses the rule in the [local LLM memory calculator](https://aiagents.org.uk/local-llm-memory-calculator/): macOS lets a model use about 75% of memory, and the conversation needs 2 to 4 GB on top. "Comfortable" leaves 4 GB spare, "Tight" leaves 2 GB. Good-for labels are adapted from [ModelFit's hardware dataset](https://github.com/modelfit-io/modelfit-hardware-dataset) (CC BY 4.0).

Prices and availability change often. Check the vendor before you buy. Spotted something out of date? [Tell me](https://aiagents.org.uk/contact/) or open an issue.

## Using the data

See [TERMS.md](TERMS.md). In short: quote it, cite it and chart it freely with a link back to the source page; don't republish the whole dataset or sell it.

Cite as: Vane, A. (2026). *UK AI prices, availability and local LLM fit.* aiagents.org.uk. https://aiagents.org.uk/open-data/
