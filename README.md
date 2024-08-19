# Missing Building Blocks in the Agent World

["AI Agents will likely be the most impactful technology of our generation"](https://transitivebullsh.it/ai-agents). In this document I present you the following modular building blocks, fully open source. Beware that most of it is still a work in progress! See this [high level overview](#highlevel-actionschema) for the current status.

## Agent OpenAPI

Turn any API into an Agent, Turn any Agent into an API.

The Agent OpenAPI serves an OpenAPI for talking to an agent, so it can be discovered publicly, and can be used as a tool for other agents. More information in the [Agent OpenAPI GitHub](https://github.com/CodeFromAnywhere/agent-openapi)

![](agent-openapi.drawio.png)

## Agent Relay

Agents need to be accessible from anywhere. The Agent Relay makes agents accessible from messaging apps, VoIP and phonecalls, and over email! Check out the [Agent Relay on GitHub](https://github.com/CodeFromAnywhere/agent-relay)

![](agent-relay.drawio.png)

## CRUD OpenAPI

Data needs to be discoverable as tools. A reliable CRUD Agent is extremely useful. [More info here](https://github.com/CodeFromAnywhere/crud-openapi)

![](crud-agent.drawio.png)

# Why

- We're living through a technological paradigm shift that will change how we interact with computers, and how humans can find purpose. A new foundation is being created now. In this important time, I want to do my part setting good standards for HMC that benefits humanity.
- Big tech capitalism is trying to create a controlled closed ecosystem for AI. As AGI is approaching, misaligned commercial incentives become ever more extreme, and I don't want to live in this walled garden distopia. The solution is an open, accessible, modular ecosystem for AI Agents. An ecosystem without any vendor lock-in or privacy problems. An ecosystem where we, the people, stay in control.

# Strategy

**ActionSchema** for _Devs_: **OEF**

- Devs want _Open_ source. Give it.
- Devs want _Easy_: Serve it BYOK, accessible, and useful.
- Devs want _Freedom_. Provide them agents so they can go Screenless.

# Key insights

- A dependency to the above is what I call "OpenAPI-first development". It is an opinionated way of [design-first](https://swagger.io/blog/code-first-vs-design-first-api/) development where your OpenAPI serves as the SSOT for a lot of things, and you don't generate it, you rather generate pieces in your code FROM it.
- Most AI is focused around realtime co-pilots because we're all still used to the direct HMC. Try making ambient pilots that don't need to be fast.
- Pick my focus. Big topics like browser automation APIs and video editing are done by hundreds of companies and are extremely hard to stay competitive in; It's a never-ending cat and mouse game.
- Products and APIs change all the time. Instead of choosing to spend knowledgework time in specific niches, index all available capabilities.
- Most users care about their privacy and would want to have things ran locally. However, running locally is hard to setup and scale. Another way to have practical privacy is to keep the core local, but run smaller fleeting tasks in the cloud.
- How any API works exactly doesn't need to be abstracted away from. The only thing we need to do is determine API capability, quality, speed, cost, and availability.

# Let's Code From Anywhere!

Welcome to [Code From Anywhere](https://codefromanywhere.com/) - a group of distributed developers and entrepreneurs building planet-first & humane-centered software. We work remotely but often come together in places like Nepal and Brazil, going on adventures.

We 🤍 Developers, AI Startups & Adventurers. Do you have a question, comment, or want to connect? Head over to our [Discord](https://discord.gg/56yJzjJjHu)

# License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## Commercial License

If your company generates more than $1,000,000 in Annual Recurring Revenue (ARR), you are required to obtain a commercial license. Please see the [COMMERCIAL_LICENSE](COMMERCIAL_LICENSE.md) file for more information.

## Contact

For commercial licensing inquiries, please contact Wijnand at wijnand AT karsens DOT com
