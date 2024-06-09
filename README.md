# Let's Code From Anywhere!

Welcome to [Code From Anywhere](https://codefromanywhere.com/) - a group of distributed developers and entrepreneurs building planet-first & humane-centered software. We work remotely but often come together in places like Nepal and Brazil, going on adventures.

We 🤍 Developers, AI Startups & Adventurers. Do you have a question, comment, or want to connect? Head over to our [Discord](https://discord.gg/56yJzjJjHu)

# Key focus: Reliable Agents by intelligent search

- Analysing thousands of services on capability, quality, speed, cost, and availability.
- Have a scalable way to sign up and get access to all service providers with multiple accounts.
- Proxy them into my own gateway which can be made available as a "Universal API" that exposes all services through a single endpoint.

Strategy: **ActionSchema** for _Devs_: **OEF**

- Devs want _Open_ source. Give it.
- Devs want _Easy_: Serve it BYOK, accessible, and useful.
- Devs want _Freedom_. Provide them agents so they can go Screenless.

**ActionSchema in different keywords: AI Software Engineer, Universal API, Reliable Agents, OLAM**

TODO: Keep jumping between these projects and aim to finish them asap. **Laserfocus**.

LONGTERM: Keep these stable services for decades. Keep LOC/Complexity LOW.

# Highlevel

This is the current ecosystem of projects developed by Code From Anywhere (❗️ dependency, 🚫 blocked, 🔴 not started, 🟠 work in progress, 🟢 done)

| Website                                                        | Purpose                                         | Status | POC                                                                                                                                                      | LOC  |
| -------------------------------------------------------------- | ----------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- |
| [Agent Relay](https://github.com/CodeFromAnywhere/agent-relay) | Make agent available anywhere                   | 🟠     | 🟢 Browser & Phonecall STS<br>🟢 Custom agent compatibility<br>🟢 Whatsapp, SMS, Messenger<br>🔴 Email<br>🔴 Deepgram STS Tool use                       | 1175 |
| User OpenAPI                                                   | Add User Management to your OpenAPI             | 🔴 ❗️ | Serve Clerk on https://login.actionschema.com and proxy+extend an OpenAPI                                                                                |      |
| [Combination Proxy](https://proxy.actionschema.com)            | Combine multiple OpenAPIs into one              | 🔴     | 🟠 Serve with form to make your own easily.<br>🔴 Examples of agents.                                                                                    | 1300 |
|                                                                |                                                 |        |                                                                                                                                                          |      |
| [Agent OpenAPI](https://agent.actionschema.com)                | Turn any API into an Agent                      | 🚫     | 🟢 Simple POC<br>🟢 OpenAPI-centric Refactor<br>🚫 Threads<br>🔴 Files<br>🔴 Agent-Agent                                                                 | 1984 |
| [CRUD OpenAPI](https://data.actionschema.com)                  | Turn database into agent-tools                  | 🚫     | 🟢 CRUD Only firsst<br>🟢 Semantic search<br>🔴 CLI<br>🚫 Config: user separation<br>🔴 ActionSchema integration<br>🔴 CRUD-Agent                        | 4450 |
| [Enhancement Proxy](https://openapi.actionschema.com)          | Allow agents to iteratively improve their tools | 🚫     | 🚫 Finish ActionSchema Rewrite<br>🟠 Serve on subdomain with frontpage<br>🔴 Create OpenAPI to self-modify                                               | ±2k  |
| [OpenAPI Explorer](https://explorer.actionschema.com)          | Explore OpenAPI Possibilities                   | 🔴     | 🟢 Forms<br>🟢 Page-per-tag, all forms on tagpage.<br>🔴 manual entry<br>🔴 Aggregate openapis from multiple endpoints<br>🔴 Expose LLM search endpoint. | 664  |

A dependency to the above is what I call "OpenAPI-first development". It is an opinionated way of [design-first](https://swagger.io/blog/code-first-vs-design-first-api/) development where your OpenAPI serves as the SSOT for a lot of things, and you don't generate it, you rather generate pieces in your code FROM it. Here are some libraries I've made to allow for this.

| Library                                                                      | Purpose                                                    | Status                                                                                            | LOC  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ---- |
| [openapi-util](https://github.com/CodeFromAnywhere/openapi-util)             | Utilities for working with OpenAPI and serving them        | 🟢 make `resolveOpenapiAppRequest`<br>                                                            | 1517 |
| [react-openapi-form](https://github.com/CodeFromAnywhere/react-openapi-form) | Auto-generate forms based on an OpenAPI                    | 🟢 Works, including Type Safety and editability<br>🟠 Include component for showing all endpoints | 838  |
| [actionschema](https://github.com/CodeFromAnywhere/ActionSchema)             | Extension of JSON Schema allowing data-centric development | 🟠 Rewrite to v2 in progress<br>🔴 x-proxy<br>🔴 x-schema<br>🔴 x-code<br>                        | 2904 |

If I feel _fancy_, work on this. More experimental:

| Website              | Purpose                      | Repo               | Status     | POC or next steps                                                 | Depends on                      |
| -------------------- | ---------------------------- | ------------------ | ---------- | ----------------------------------------------------------------- | ------------------------------- |
| OpenAPI Tester       |                              |                    | Big Wish   | E2E testing/validating an OpenAPI's functionality                 | ActionSchema                    |
| oAuth2 Authenticator |                              |                    | Big Wish   | Automatic signup, login, and payments to gather API access        | serverless-browser              |
| Serverless Browser   |                              | serverless-browser |            | Serverless Playwright Browsing OpenAPI                            |                                 |
|                      |                              |                    |            |                                                                   |                                 |
|                      |                              | procedures         | Brainstorm | Natural Language to Operations mapping                            | Good OpenAPI search             |
|                      |                              |                    | Brainstorm | LLM Hierarchy Creation, Maintenance, and Search                   |                                 |
| ActionSchema Demo    | Show how ActionSchema works  | actionschema-demo  | Paused     | VSCode plugin for OpenAPI selection and form-filling              | Functional OpenAPI              |
|                      |                              |                    | Big Wish   | Slow-agents that can continue very long or self-activate          | ActionSchema                    |
| Universal API        | Universal-API or Open-LAM    |                    |            | Exposes all services through a single cacheable NLP endpoint      | OpenAPI Explorer, Search, Proxy |
| Human OpenAPI        | Turn people into agent-tools |                    | Blocked    | User can signup after which the API can communicate with the user | 🟢 Agent Relay, 🔴 User OpenAPI |

# Key insights

- Most AI is focused around realtime co-pilots because we're all still used to the direct HMC. Try making ambient pilots that don't need to be fast.
- Pick my focus. Big topics like browser automation APIs and video editing are done by hundreds of companies and are extremely hard to stay competitive in; It's a never-ending cat and mouse game.
- Products and APIs change all the time. Instead of choosing to spend knowledgework time in specific niches, index all available capabilities.
- Most users care about their privacy and would want to have things ran locally. However, running locally is hard to setup and scale. Another way to have practical privacy is to keep the core local, but run smaller fleeting tasks in the cloud.
- How any API works exactly doesn't need to be abstracted away from. The only thing we need to do is determine API capability, quality, speed, cost, and availability.

## Questions

- Can ActionSchema become agentic: allowing an agent to decompose tasks in parallel and sequential ways?
- How can I build a meta programming language that dynamically finds new actions, tests them, and improves them, that can create purpose-oriented change in a system?
  - How can I measure purpose-oriented change and figure out whether it's worth the cost?

# Contributors and Sponsors

Top contributors

- [Wijnand Karsens](https://karsens.com)
- lonely here... 👀

# License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## Commercial License

If your company generates more than $1,000,000 in Annual Recurring Revenue (ARR), you are required to obtain a commercial license. Please see the [COMMERCIAL_LICENSE](COMMERCIAL_LICENSE.md) file for more information.

## Contact

For commercial licensing inquiries, please contact Wijnand at wijnand@karsens.com
