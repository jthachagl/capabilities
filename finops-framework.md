Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
[work in progress]

# FinOps Framework
## A unified framework for building an effective practice in an Enterprise

The framework provides a roadmap to implement FinOps:

- Defines the Capabilities required for the entire practice
- Segments them by Persona and Function driven by SIG inputs (finance, eng, kubernetes, etc)
- KPIs are attached to measure effectiveness in each area and—where relevant—each capabilit
- Responsibilities are rolled up to a RACI of ownership

## TAC's primary output becomes the Framework

- Each portion of the framework is owned by a SIG (finance, eng, kubernetes, etc)
- SIG inputs drive continuous improvement of framework
- SIGs recommend quarterly (TBD) updates to the framework to the TAC via Github pull request
- TAC votes quaterly (TBD) to approve framework updates and merges them to master Framework branch

## Framework drives Certification requirements

- Learning objectives for certifications are attached to each area/capability set
- Training curriculums are driven by those learning objectives
- Training materials are built by FinOps or others to support the learning objectives

## FinOps Certifications verify an understanding of the framework

- Persona based certifications hosted by the Linux Foundation 
- SIGs define what each persona needs to know
- That knowledge is translated into exam questions
- LF/FinOps work with training partners to develop content to teach the framework

## Benchmarking of capabilities and KPIs

- Survey/data (SIG?) supports benchmarking capabilities on an effective practice
- Anonymized, crowdsourced KPI data allows enterprises to measure against "what great looks like"

## FinOps Framework output

- Framework master updates are ouputted into a rich HTML documentation experience like https://www.gatsbyjs.com/tutorial/
- Outputs would fall into a taxonomy that enables filtering the experience for persona (e.g., Finance vs. Eng) and Clouds (e.g. AWS vs GCP) like https://www.balena.io/docs/learn/getting-started/raspberrypi3/nodejs/

## Community support enables contribution and learning

FinOps Foundation is an aggregator and enabler of discussion and evolution of the practice.

- Slack channels tie to Framework areas and drive inputs to SIG updates
- Centralized view into regional, topical and persona based events (meetups, vendor discussions, FinOps member meetings)
- IdeaExchanges drive live discussion forums for sharing of best practices via Zoom breakout rooms
- Community discussions drive improved framework, each event's takeaways captured and integrated

## FCP, FCSP, FTP partners enable implementation of the Framework

- Tooling supports accomplishment of capabilities: whether SaaS or Open Source
- Some capabilities are internal muscle, some are software, some are services
- Vendors and consultancies are mapped against the capabilties of the Framework 
- Practitioners can use that mapping to find help for areas where they are weak

To qualify for the FinOps Certified program a vendor needs to provide solutions for a specific number of capabilities. Each checked line item adds to the total score. The exact amount of capabilities a vendor needs to support to certify will change / increase over time as the industry matures (requirements to be defined by the TAC). Vendor members work to be the best at providing solutions to the capabilties in the framework. E.g. Platforms, Service Providers, Training Partners. 

# FinOps Framework v0.1

## Pillars

- [Visibility And Allocation](#visibility-and-allocation)
- [Rate Reduction](#rate-reduction)
- [Cost Avoidance](#cost-avoidance)
- [Benchmark Performance](#benchmark-performance)
- [Enable Real-Time Decision Making](#enable-real-time-decision-making)
- [Align Plans to the Business](#align-plans-to-the-business)

## Visibility And Allocation

- [ ] Multi-cloud ingestion and normalization of spend data across a minimum of AWS, Azure, and GCP
- [ ] Cloud cost visualization supports aggregation and filtering e.g. product, account, time, tag
- [ ] Allow mapping of cloud resources (a.g. accounts, projects) to your organization's structure
- [ ] Align cloud decision makers with FinOps goals
- [ ] Customizable dashboards to visualize amortized costs and forecasted spend
- [ ] Cost visualization caters to different levels in the organization e.g. executive versus leadership versus engineer
- [ ] Cost data is up-to-date, meaning less than 2 days old
- [ ] Support amortization of prepayment products (Committed Use Discounts, Reservations, Savings Plans)
- [ ] Accurate and dynamic calculation of custom rates, shared costs and amortization metrics
- [.] Shared cost allocation based on fixed, proportional or even distributions
- [ ] Create showback and chargeback reporting
- [ ] Support fully loaded costs incl. enterprise discounts, private pricing agreements, support fees, costs for site licenses etc.
- [ ] Define tagging strategy and support management of tagging rules
- [ ] Manage tagging compliance e.g. enforcement, alerting, and auto correction
- [ ] Define budgets and report actual versus budget
- [ ] Define forecasts and report forecast versus actual variance
- [ ] Alert and visualize budget overages
- [ ] Alert and visualize cost spikes that may not be large enough to impact budgets
- [ ] Support FinOps program tracking through e.g. program specific KPIs
- [ ] Able to provide visibility into how your organization performs across the industry

### KPIs:

- % of spend that can be fully allocated
- % of forecast to actual variance over specific periods
- * % untagged resources
- % wrongly tagged resources
- % total tag coverage
- % taggable items tagged
- % of spend that is untaggable 
- Hours between cost incurred and cost displayed to end team
- Frequency of cost data updates
- Avg price per hour of compute
- Unit cost (spend divided by a business metric)

## Rate Reduction

- [ ] Visualize effect of enterprise discounts, private pricing agreements
- [ ] Visualize effect of custom discounts, volume discounts
- [ ] Visualize, report, and track the effect of sustained usage discounts
- [ ] Track commitment for enterprise discounts, private pricing agreements over time and show remaining commitment for each agreement
- [ ] Recommend optimizations to existing licensing portfolio
- [ ] Visualize coverage and utilization of prepayment products (Committed Use Discounts, Reservations, Savings Plans) and show trending over time
- [ ] Analyze effectiveness of existing prepayment portfolio and provide improvement recommendations
- [ ] Recommendations allow balancing of various rate types
- [ ] Select discounts that match your flexibility
- [ ] Utilize the marketplace when making recommendations
- [ ] Provide purchase recommendations for prepayment products (Committed Use Discounts, Reservations, Savings Plans)
- [ ] Recommendations are aware of seasonality
- [ ] Recommendations are aware of auto scaling workloads
- [ ] Visualize, recommend, manage, and track capacity reservations

### KPIs

- RI Coverage
- Savings Plan Coverage
- Committed Use Discount coverage
- Custom pricing commitment tracking

## Cost Avoidance

- [ ] Visualize, recommend, and track right-sizing opportunities within a compute family
- [ ] Visualize, recommend, and track right-sizing opportunities across compute families
- [ ] Allow user prompted remediation of right-sizing opportunities
- [ ] Submit pull requests for right-sizing recommendations
- [ ] Leverag Continuous Integration/Continuous Delivery (CI/CD) automation for cost avoidance
- [ ] Able to benchmark the performance of cloud workloads
- [ ] Visualize, recommend, manage, and track cloud parking opportunities
- [ ] Visualize, recommend, and track unrealized savings opportunities (underused, unused, orphaned resources)
- [ ] Allow user prompted remediation of unrealized savings opportunities (underused, unused, orphaned resources)
- [ ] Auto remediate unrealized savings opportunities (stopping of unused resources, deletion of orphaned resources, data lifecycle management)
- [ ] Visualize and track realized cost avoidance opportunities
- [ ] Provide visibility into container utilization e.g. node utilization, pod utilization
- [ ] Report, track, manage, and enforce red / green zone policies
- [ ] Alert, report, track, manage, and enforce policies and governance in the cloud

### KPIs

- Rightsizing opportunity value
- Usage on weekends vs weekdays
- % of spot vs other coverage
- % orphaned EBS volumes
- % orphaned snapshots
- Aged snapshots
- Idle instances > 30-days
- Idle instances < 30-days

## Benchmark Performance
- [ ] Trending & Variance Analysis
- [ ] Create Scorecards, metrics & KPIs
- [ ] Benchmark internally and against “industry” peers

## Enable Real-Time Decision Making
- [ ] Provide timely and consistent spend / usage data to all stakeholders
- [ ] Identify Anomalies based on machine learning 
- [ ] Find & Remove underutilized services

## Align Plans to the Business
- [ ] Mini-Business Cases
- [ ] Tracking and Trending
- [ ] Communication strategy
- [ ] Ongoing reviews with stakeholders on optimization opportunities
- [ ] Develop a framework for decision making that aligns with the business drivers

## Access and Permissions

- [ ] Integration with SSO
- [ ] Ability to focus or restrict visibility and features based on role
- [ ] Ability to limit scope of access by tags, departments, users, or business logic constructs

## Collaboration and Communication Capabilities
- Foster communication and collaboration among operations, development, and finance teams
- Deliver data and insights to team workflows such as ticketing systems like JIRA or ServiceNow
- Provide acknowledgement and status of recommendations bi-directionally between systems

## Container Capabilities
- [ ] ETL of container usage married to infrastructure cost data
- [ ] Allocation of container spending based on defined taxonomy of tags, labels, namespaces, etc
- [ ] Optimization of container usage
- [ ] Integration of container cost data with traditional IaaS spending for complete costs

## Finance Capabilities
tbd to breakout or categorize in to other areas

## Engineering Capabilities
tbd to breakout or categorize in to other areas

## Automation Capabilities
tbd to breakout or roll in to other areas

## Software License Management Capabilities
tbd name (SAM, SaaS, etc)