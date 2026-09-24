# Master experiences

This file is the library of STAR stories for cover letters. `resume.typ` holds the public record. This file holds the stories behind it. Add a story when it is true. Do not invent metrics, tools, or outcomes.

## Motivation

- Yin studies computer science with a commerce minor because he wants to see how a business runs and stays profitable, then contribute to that as a software engineer.
- Financial accounting made that concrete: the numbers depend on the systems that record and check them.
- He wants to apply what he is learning in his finance and business operations courses on the job.

## VoltSafe — server monitoring

- **Situation:** VoltSafe hosted its main web dashboards and Postgres databases on AWS EC2, and the team usually found problems after something had already broken.
- **Task:** Collect CPU, disk, and RAM for those servers and show the readings in the internal admin dashboard.
- **Action:** Yin deployed a lightweight Docker collector on each EC2 instance that exposed hardware metrics on a REST endpoint.
- **Action:** A central Prometheus server scraped those endpoints and stored them as a time series with a rolling two-week retention window, which kept storage cost down.
- **Action:** He drew the charts in React inside the existing dashboard by polling the Prometheus REST API, so the team did not have to open Grafana.
- **Result:** Over five months the view warned the team more than five times before a failure.
- **Result:** One instance hit 95% disk, and the team expanded storage before it crashed.
- **Result:** The team moved from reacting to outages to catching them first.

## CreateYourStory — flatter story schema

- **Situation:** Gemini models ignored a nested, recursive story schema. Stories stayed one or two levels deep, nodes had only one or two choices, and ending flags were almost never set.
- **Situation:** Switching models, raising the thinking level, removing the token limit, and adding an example tree to the prompt did not fix it.
- **Task:** Generate a choose-your-own-adventure in one pass that is three or four levels deep, gives each node two or three choices, marks endings, and has exactly one winning path.
- **Action:** Yin replaced the recursive schema with a flat dictionary of nodes keyed by id, where each node points at its choices by id.
- **Action:** He treated a node with an empty choice list as an ending, so the model no longer had to set an ending flag.
- **Result:** On a medieval theme with Gemini 3.5 Flash, the output went from 3 nodes and no winning ending to 16 nodes, two to four levels deep, with exactly one winning ending.

## CPSC 310 — REST Client lesson

- **Situation:** Many students in Yin's CPSC 310 lab had no prior software engineering experience and tested project endpoints through the frontend or by hand.
- **Task:** Help them test the project's REST API quickly.
- **Action:** He volunteered a presentation on Huachao Mao's REST Client extension for VS Code.
- **Result:** Students could call the endpoints directly.
