# Mintbase Grant Proposal

## Project Overview :page_facing_up:

If this application is in response to an RFP, please indicate this on the first line of this section.

If this is an application for a follow-up grant (the continuation of an earlier, successful Mintbase grant), please provide name and/or pull request of said grant on the first line of this section.

### Overview

Please provide the following:

- If the name of your project is not descriptive, a tag line (one sentence summary).
- A brief description of your project.
- An indication of how your project relates to / integrates into the Mintbase / NEAR ecosystem.
- An indication of why your team is interested in creating this project.

### Project Details

We will create simple API, which allows to integrate functionality in different products (ex. Mintbase UI, Telegram Bot or other) 
- API specification: https://www.notion.so/gusevvladimir/Projects-with-potential-power-users-7982033da4424787993fed3001a7f54a
- MVP: Telegram bot: @metronomo_bot
- Technology stack to be used: Google Cloud Functions, Google Cloud Storage, Python

### Ecosystem Fit

Help us locate your project in the Mintbase landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
- Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?
- What need(s) does your project meet?
- Are there any other projects similar to yours in the Mintbase / NEAR ecosystem?
  - If so, how is your project different?
  - If not, are there similar projects in related ecosystems?

## Team :busts_in_silhouette:

### Team members

- Name of team leader
- Names of team members

### Contact

- **Contact Name:** Full name of the contact person in your team
- **Contact Email:** Contact email (e.g. john@duo.com)
- **Website:**

### Legal Structure

- **Registered Address:** Address of your registered legal entity, if available. Please keep it in a single line. (e.g. High Street 1, London LK1 234, UK)
- **Registered Legal Entity:** Name of your registered legal entity, if available. (e.g. Duo Ltd.)

### Team's experience

Please describe the team's relevant experience. If your project involves development work, we would appreciate it if you singled out a few interesting projects or contributions made by team members in the past. For research-related grants, references to past publications and projects in a related domain are helpful.

If anyone on your team has applied for a grant at the Mintbase previously, please list the name of the project and legal entity here.

### Team Code Repos

- https://github.com/Metronomo-xyz

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/<person_1>
- https://www.linkedin.com/<person_2>

## Development Status :open_book:

As we are going to create infrastructure protocol for creating user acquisition tools for web3, currently we are aiming to create first valuable tools and infrastructure and technology they need.

We believe that MVP will help us to both provide value for projects on NEAR ecosystem and create foundation for user acquisition infrastructure protocol.

As for now we've already done:
1. Telegram Bot to test hypothesis on NEARCON and research projects pains and value request. We've found out that user acquisition part of ecosystem lacks most of familiar tools and techniques.
2. For now we consider, that main method to find power users will be RFM-segmentation https://en.wikipedia.org/wiki/RFM_(market_research)
3. We've created very basic projects and users similarity analysis tools and found out, that it's possible to compute on net very expensive servers and in reasonable time for creating product.
4. There are several users-similarity techniques described in papers, which we're going to try and implement. For example (but not limited to):
   1. https://link.springer.com/article/10.1007/s10115-021-01651-8
   2. https://ieeexplore.ieee.org/abstract/document/904471
   3. https://link.springer.com/chapter/10.1007/978-981-19-1018-0_42

During this project we are going to get 3 main results:
- create module to find power users. interacted with given smart contract.
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

In the future, we are looking forward:
- generalize power-user analysis module to be possible to use as separate opne-source product
- rewrite data extraction module (not covered by this grant application) to user NEAR Lake data (for Google Cloud) instead of NEAR Indexer for Explorer data
- receive feedback on value of created features and adjust roadmap of future work
- create recommender system for NFT marketplaces
- blend web2 & web3 data to enhance user acquisition

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** NEARCON 2022