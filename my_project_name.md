# Mintbase Grant Proposal

- **Project Name:** Metronomo
- **Team Name:** Metronomo Team
- **Payment Address:** metronomo.near
- **[Level](../README.md#level_slider-levels):** 2

## Project Overview :page_facing_up:

### Overview
[https://metronomo.xyz/](Metronomo) is a cross-chain user growth infrastructure

#### Problem
We asked a bunch of web3 projects about their biggest challenges. All of them mentioned user acqusition as an urgent issue.
That's how we had started building "hubspot for web3". But from the very beginning we faced 2 problems:
1. On-chain data is fragmented and poorly structured to create user profiles 
2. ETL and mapping is resource intensive and expensive

#### Solution
We decided to create basic data layer for building marketing tools:
- structure and combine on-chain data into users, projects, transactions and other relevant dimensions
- provide API to access and manage data
- give fundamental technologies for building martech products (e.g. NFT recommendation and personalization system, matching web2 and web3 user data, zero, 1st, 2nd & 3rd party data system, knowledge and social graph and others)

#### Why we do
- Our team has 10+ year experience in digital marketing, data science, development and data engineering.
- We are highly confident that on-chain data has an extremely important role in scaling web3 products and ecosystem as a whole.
- So we see our mission as **make web3 martech great by the next bull run**

### Project Details

We will deliver easy to use API, which allows to integrate functionality in different products (ex. Mintbase UI, Telegram Bot or other) 
- API specification: https://www.notion.so/gusevvladimir/Projects-with-potential-power-users-7982033da4424787993fed3001a7f54a
- MVP: Telegram bot: [@metronomo_bot](https://t.me/metronomo_bot)
- Technology stack to be used: Google Cloud Functions, Google Cloud Storage, Python

### Ecosystem Fit
#### Where and how does your project fit into the ecosystem?
We see Metronomo as the user growth module of Mintbase now and part of marketplace contract 2.0 in the next iteration

#### Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?
Mintbase ecosystem projects

#### What need(s) does your project meet?
As the part of marketplace contract 2.0 allow merchants to create product selections based on user profiles and similarity to other projects to grow revenue

#### Are there any other projects similar to yours in the Mintbase / NEAR ecosystem?
All existing NEAR products cover a single aspect of user growth, but are not open source infrastructure
(e.g. Wombi - dashboards, Datrics - creating ML models, Plex - user profiling and engaging)

#### If so, how is your project different?
We build open source user growth infrastructure protocol

#### If not, are there similar projects in related ecosystems?
0xscope, The Graph, Permission.io and other infrustruce products are close but no completely similar
They are focused on general indexing issue, but not on marketing data needs

## Team :busts_in_silhouette:

### Team members

- Vladimir  Gusev (team leader)
- Yaroslav Bondarchuk
- Vadim Smirnov

### Contact

- **Contact Name:** Vladimir  Gusev
- **Contact Email:** vladimir@metronomo.xyz
- **Website:** https://metronomo.xyz/

### Legal Structure

- **Registered Address:** -
- **Registered Legal Entity:** -

### Team's experience
**Vladimir Gusev**:

- co-Founder and CEO at [Metronomo](https://metronomo.xyz/)
- ex-Partner & VP of Growth and later COO at [GigAnt - largest Workforce-as-a-Service marketplace in CIS](https://gigwork.ru/)
    - Company was successfully acquired by [Avito - World’s Most-visited Classified Ads Site by Similarweb](https://www.yahoo.com/lifestyle/avito-named-world-most-visited-190600803.html)
- ex-Co-founder and CMO at Russia’s TOP10 Digital Marketing Agency
    - Company was successfully acquired by TOP1 digital marketing group
- ex-Professional online poker player since 2005 till 2010


**Yaroslav Bondarchuk**

8+ years in analytics, data science and data engineering:
- co-Founder and CPO at [Metronomo](https://metronomo.xyz/)
- ex-Head of analytics at [GigAnt - largest Workforce-as-a-Service marketplace in CIS](https://gigwork.ru/)
- ex-Product owner at [Retail Rocket](https://retailrocket.net/) (recommender system product)
- ex-Head of analytics at [Skillbox - leading edtech platform in Eastern Europe](https://skillbox.com/)

**Vadim Smirnov**

9+ years in marketing and product growth:
- co-Founder and CMO at [Metronomo](https://metronomo.xyz/)
- ex-Head of growth at [GigAnt the - largest Workforce-as-a-Service marketplace in CIS](https://gigwork.ru/)
- Advisor at [Sailplay - international marketing automation platform](https://sailplay.com/)
- ex-Performance marketing group head at [Skillbox - leading edtech platform in Eastern Europe](https://skillbox.com/)

### Team Code Repos
https://github.com/Metronomo-xyz

### Team LinkedIn Profiles (if available)

- [Vladimir Gusev](https://www.linkedin.com/in/gusevv1987/)
- [Yaroslav Bondarchuk](https://www.linkedin.com/in/bondarchukyaroslav/) 
- [Vadim Smirnov](https://www.linkedin.com/in/vadim-smirnov-71a66b189/)

## Development Status :open_book:

We are building infrastructure protocol for creating user growth tools for web3. Currently we are aiming to create first valuable tools, infrastructure and technology they need.

We believe that MVP will help us both provide value for projects in Mintbase ecosystem and create foundation for user acquisition infrastructure protocol.

As for now we've already done:
1. [Telegram Bot: @metronomo_bot](https://t.me/metronomo_bot) to test hypothesis on NEARCON and research projects pains and value request. We found out that user acquisition part of ecosystem lacks most of familiar tools and techniques.
2. For now we consider, that main method to find power users will be RFM-segmentation https://en.wikipedia.org/wiki/RFM_(market_research)
3. We created very basic projects and users similarity analysis tools and found out, that it's possible to compute on net very expensive servers and in reasonable time for creating product.
4. There are several users-similarity techniques described in papers, which we're going to try and implement. For example (but not limited to):
   1. https://link.springer.com/article/10.1007/s10115-021-01651-8
   2. https://ieeexplore.ieee.org/abstract/document/904471
   3. https://link.springer.com/chapter/10.1007/978-981-19-1018-0_42

During this project we are going to get 3 main results:
- create module to find power users, interacted with given smart contract.
- create module to calculate users similarity measure and find potential power users
- create module to find smart-contract which potential power users interact with

## Development Roadmap :nut_and_bolt:

### Overview

- **Total Estimated Duration:** 3,5 months
- **Full-Time Equivalent (FTE):**  5 FTE
- **Total Costs:** 25,000 USD

### Milestone 1 — Implement power-users search module

- **Estimated duration:** 1 month
- **FTE:**  1
- **Costs:** 5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | proprietary
| 0b. | Documentation | We will provide both **inline documentation** of the code and basic tutorial on how to deploy and run created module.
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 1. | Power-users-search module | We will create a module that will search for power users of a smart contract, given the indexed blockchain data in described format.  


### Milestone 2 - Implement look-a-like module

- **Estimated Duration:** 1,5 months
- **FTE:**  2
- **Costs:** 15,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | proprietary
| 0b. | Documentation | We will provide both **inline documentation** of the code and basic tutorial on how to deploy and run created module.
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 1. | Look-a-like module | We will create a module that will create look-a-like (embeded vector) representation of a power users in user space

### Milestone 3 - Implement users similarity module and users activity module

- **Estimated Duration:** 1 month
- **FTE:**  1
- **Costs:** 5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | proprietary
| 0b. | Documentation | We will provide both **inline documentation** of the code and basic tutorial on how to deploy and run created module.
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article** and perform a workshop that explains how to use created API and how to receive value from this product.
| 1. | Users similarity module | We will create a module that will find most similar users in whole NEAR blockchain given specific set of look-a-likes
| 2. | Similar contracts search module | We will create module that will find and count how many potential similar to look-a-like users interacted with each smart contract (with at list 1 interaction during given past period)
| 3. | API setup | We will run an API, which Mintbase users or Mintbase itself can use or integrate in Mintbase UI

## Future Plans

In the future our main goal is to develop protocol architecture and economics concept based on user research.
Protocol should allow to build tools like (but lot limited to):
- Recommender system for NFT marketplaces
- Personalized user incentives
- Affinity analysis
- Product analytics tools
- Open-source zero-party tracker
- Competitor analysis
- Cohort analysis
- etc.

Our roadmap includes delivering:
- Generalized power-user analysis module that can be used as separate open-source product
- Rewrited data extraction module (not covered by this grant application) to user NEAR Lake data (for Google Cloud) instead of NEAR Indexer for Explorer data
- Blend web2 & web3 data to enhance user acquisition
- Provide API to access and manage marketing data

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** 

from Paul Kuveke at NEARCON 2022
