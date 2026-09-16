# `openapi-openhack`

## Concept

`openapi-openhack` is the reference repository for a new experimental community initiative around Openapi.

Openapi's APIs are primarily professional and enterprise services. They solve problems involving electronic invoicing, certified email, postal services, digital signatures, timestamps, company information, vehicles, real estate, cadastral information, risk assessment and other specialized services.

These APIs were not designed for hobbyists.

**That's exactly the point.**

OpenHack asks a different question:

> What happens when we give hobbyists, hackers, makers and curious developers access to capabilities they would normally never have a reason to use?

The objective is not to turn hobbyists into Openapi customers.

The objective is to let them **play with serious infrastructure**.

---

# The target: the weekend hacker

OpenHack is not primarily aimed at enterprise developers evaluating an API for their company.

The target is the developer who builds things because building things is fun.

The person with:

* a Raspberry Pi sitting somewhere at home;
* an old computer that still works;
* a €5 VPS;
* a homelab;
* an unfinished side project;
* a weird GitHub Action;
* a bot nobody asked for;
* a domain bought for an idea that never shipped;
* a new programming language they are learning for no practical reason;
* an AI coding agent helping them build something on Saturday night.

They may be professional developers, students, sysadmins, researchers, electronics enthusiasts or simply curious people.

What matters is not their profession.

What matters is the attitude:

> **Nobody asked me to build this. I just wanted to see if it could be done.**

---

# Why now

Writing software is becoming dramatically cheaper.

A developer with modern open-source software, GitHub and AI coding tools can create in hours what previously required days or weeks.

For many small applications, the code itself is no longer the scarce resource.

What remains scarce are **capabilities outside the computer**.

An AI can write the code for sending a certified email.

It cannot provide the certified email infrastructure.

An AI can implement a company search interface.

It cannot invent authoritative company information.

It can write software dealing with vehicles.

It cannot independently know real information associated with a vehicle.

It can calculate hashes.

It cannot independently certify that a document existed at a particular moment.

It can generate a PDF.

It cannot physically deliver a letter somewhere in Italy.

This creates an interesting division:

> **Open source and AI provide the software.
> Specialized services provide access to the real world.**

Openapi already operates precisely in this second layer.

---

# Enterprise APIs as hacker material

Normally these capabilities are used inside serious workflows:

* invoicing systems;
* large e-commerce platforms;
* automotive businesses;
* document workflows;
* legal processes;
* company verification;
* real-estate platforms;
* communication infrastructure.

A hobbyist probably doesn't *need* them.

OpenHack does not pretend otherwise.

Instead, we treat these services the way hackers have historically treated interesting technology:

**as material for experimentation.**

Kubernetes was not created for three Raspberry Pis.

People run Kubernetes on three Raspberry Pis anyway.

Industrial electronics are not created for weekend experiments.

Makers experiment with them anyway.

Radio equipment, retrocomputers, microcontrollers, 3D printers and home automation all developed communities where experimentation itself is part of the value.

OpenHack applies the same philosophy to APIs.

---

# The principle

OpenHack should never begin with:

> "Let's build a demo for this Openapi API."

It should begin with:

> **"I wonder if we can make this happen."**

The API comes later.

A project does not need to demonstrate commercial value.

It does not need to become a startup.

It does not need to scale.

It does not need a business plan.

It does not even need to be particularly useful.

It only needs to be **interesting**.

---

# Serious APIs, unserious projects

A possible informal motto for the initiative is:

> **Serious APIs. Unserious projects.**

Another useful expression of the philosophy is:

> **Build software that touches the real world.**

Openapi provides capabilities that allow software to escape the purely computational world.

Code can cause or observe something outside itself.

For example, code may:

* send a real SMS;
* send certified email;
* send physical mail;
* timestamp a document;
* sign something;
* query real company information;
* query vehicle information;
* interact with domains;
* access real-estate or cadastral information;
* interact with specialized professional infrastructure.

These are interesting **primitives of the real world**.

OpenHack explores what people can create by combining them with open-source software, hardware, AI, old computers, strange programming languages and imagination.

---

# Not an hackathon

OpenHack should explicitly avoid hackathon culture.

No artificial 24-hour or 48-hour pressure.

No mandatory teams.

No startup pitches.

No business plans.

No requirement to create a "product".

No endless presentations to a jury.

No pressure to turn an experiment into a company.

The desired atmosphere is closer to:

* retrocomputing;
* amateur radio;
* demoscene;
* homebrew computing;
* maker culture;
* homelabs;
* hardware hacking;
* recreational programming.

People should be able to spend an evening, a weekend or three months on an experiment.

Someone may submit 40 lines of Bash.

Someone else may build a Raspberry Pi device.

Someone may create a game.

Someone may connect an API to a 30-year-old computer.

Someone may publish nothing more than an interesting proof of concept.

All are legitimate contributions.

---

# Useless is welcome

This principle should be explicit:

> **Useless is welcome.**

A useless experiment can reveal an unexpected technical possibility.

A ridiculous project can teach more than a conventional tutorial.

A project nobody would deploy in production can still contain excellent engineering.

OpenHack should reward curiosity rather than commercial usefulness.

The fundamental question is:

> **Can it be done?**

not:

> "Can we sell it?"

---

# Experiments instead of applications

The natural unit of OpenHack is therefore not necessarily an application.

It is an **experiment**.

Examples of the style of question we want to encourage:

> Can a Git commit send a physical letter?

> Can a Raspberry Pi interact with Italian bureaucracy?

> Can we prove that this source code existed today?

> Can an old computer query a modern professional API?

> Can a shell script interact with a service normally used by large companies?

> Can we turn company data into an artistic visualization?

> Can we connect a physical button to certified email?

> Can we make something happen in the physical world from a GitHub Action?

These questions are intentionally open.

The community decides what the answers look like.

---

# Openapi as a bridge to the real world

One useful conceptual model is to think of Openapi as a kind of **virtual hardware**.

A Raspberry Pi gives software GPIO pins through which it can interact with physical devices.

Openapi gives software another set of interfaces through which it can interact with external services and real-world information.

Conceptually:

```text
                    YOUR CODE

                       │
         ┌─────────────┼─────────────┐
         │             │             │
         ▼             ▼             ▼

     OPEN SOURCE      HARDWARE      OPENAPI

         │             │             │
         ▼             ▼             ▼

     computation     physical      real-world
                     devices       services/data
```

The interesting territory for OpenHack lies at the boundaries between these worlds.

---

# AI changes the game

AI coding agents make this particularly timely.

The weekend hacker no longer necessarily needs to know how to implement every component.

They can describe an idea and rapidly produce:

* a web interface;
* a CLI;
* a parser;
* a bot;
* a database;
* a Docker image;
* a GitHub Action;
* an MCP server;
* a Home Assistant integration.

The difficult part increasingly becomes:

> **What can my software actually reach?**

OpenHack gives experimentation access to capabilities that cannot simply be generated by an LLM.

The code may be cheap.

The connection to reality is not.

---

# Community model

`openapi-openhack` should be the central reference repository.

It does not necessarily contain all experiments.

Instead, it can contain:

```text
README.md
CONTRIBUTING.md

ideas/
experiments/
challenges/
examples/

docs/
  philosophy.md
  getting-started.md

.github/
  ISSUE_TEMPLATE/
```

Community projects may live in their authors' own repositories.

OpenHack can index and showcase them.

A contribution might therefore be as small as:

```yaml
name: My Ridiculous Experiment
author: @developer
repository: https://github.com/...
api:
  - timestamp
hardware:
  - raspberry-pi
description: >
  I wanted to see whether...
```

The important asset becomes the **catalogue of experiments and ideas**, rather than one monolithic codebase.

---

# OpenHack Challenges

Occasionally Openapi can propose an open-ended challenge.

Not a contest with a deadline.

More like a playground.

For example:

> **This month we're playing with timestamps.**

And one simple question:

> What would you build if your program could independently prove that something existed at a particular time?

People can respond with ideas, snippets, repositories or experiments.

Another month:

> **We're playing with Postal Service.**

Question:

> What's the strangest reason you can invent for software to send a physical letter?

There does not have to be a winner.

Pulse can simply showcase interesting results.

---

# OpenHack and Pulse

Openapi Pulse becomes the editorial amplifier for OpenHack.

Pulse can periodically highlight:

**OpenHack Experiment of the Week**

rather than:

**OpenHack Winner**

This distinction matters.

The initiative should promote exploration, not competition.

Interesting experiments can appear in:

* Pulse;
* GitHub Discussions;
* organization README cards;
* social posts;
* technical articles;
* community showcases.

A broken prototype with an excellent idea may deserve as much attention as polished software.

---

# API credits

Where economically feasible, Openapi could occasionally provide small API credits to community experiments.

The philosophy should not be:

> "We'll pay you to promote Openapi."

Instead:

> **"We'll provide the material. You experiment with it."**

This is analogous to giving development boards or electronic components to makers.

The developer retains creative freedom.

---

# What success means

OpenHack should not primarily measure:

* leads;
* enterprise conversions;
* applications shipped;
* startups created.

Useful signals are instead:

* experiments submitted;
* external repositories created;
* contributors;
* Discussions;
* forks;
* weird integrations;
* articles written by participants;
* hardware experiments;
* languages and platforms attempted;
* community members helping one another;
* unexpected uses of APIs.

The long-term commercial benefit for Openapi is indirect.

Developers discover the brand while doing something enjoyable.

Some of those developers will eventually encounter professional problems where the same services become genuinely useful.

At that moment Openapi is no longer an unknown API provider.

It is:

> **"Those people whose APIs I played with."**

That familiarity has value.

---

# Cultural rules

OpenHack should protect a few principles as it grows:

**Curiosity over usefulness.**

**Experiments over products.**

**Collaboration over competition.**

**Learning over pitching.**

**Show the code.**

**Explain what failed.**

**Small projects are welcome.**

**Old technology is welcome.**

**Strange technology is welcome.**

**Unfinished experiments are welcome.**

**Useless is welcome.**

And perhaps most importantly:

> **Don't build what we expect.**

---

# Position inside Openapi

OpenHack does not change Openapi's enterprise positioning.

Openapi continues providing serious professional services to businesses.

OpenHack represents a deliberately different relationship with the GitHub community.

The distinction can remain very simple:

> **Openapi builds serious infrastructure.
> OpenHack lets hackers play with it.**

That contrast is not a weakness.

It is the entire idea.

---

# Repository identity

Repository:

`openapi/openapi-openhack`

Working name:

**OpenHack**

Possible short description:

> **🧪 Serious APIs, unserious projects. A playground for hackers, makers and curious developers experimenting with Openapi.**

Possible longer tagline:

> **Enterprise APIs weren't made for weekend hackers. We think that's a good reason to play with them.**

The repository should feel less like developer documentation and more like the entrance to a workshop.

Not:

> "Here are our APIs."

But:

> **"Here's the workshop. What weird thing are you building?"**

---

# The central idea

OpenHack ultimately exists because of a simple observation.

Software development is becoming easier.

Open-source software provides enormous amounts of high-quality infrastructure.

AI can generate increasingly large portions of applications.

But software still needs **doors into the real world**.

Openapi owns and operates some interesting doors.

Most were built for companies.

OpenHack leaves a few of them open for curious people to play with.

> **Nobody needs to build anything.**
>
> **Nobody needs to start a company.**
>
> **Nobody needs to win.**
>
> **Come in, pick something up, and see what it can do.**
