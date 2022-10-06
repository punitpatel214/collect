# Collect
Collect is a data collection platform that is being used by customers in 35+ countries, has over 100,000 data collectors relying on it, and has powered data collection for over 11 million responses. Its features include team management, multilingual forms, and offline data collection. Our customers use Collect to power their most critical activities — from governments delivering vaccines to small business owners managing their daily inventory, to a zoo monitoring a rare wildlife species.

### Requirements
This section contains the requirements, distilled from the [provided document](https://docs.google.com/document/d/1C_VTxm3W6l4D4CyANVb6Hu5TKlZ9Ajn2ed-7h9sw84A/edit).

- **Ingestion service and primary store** : The ingestion service interacts with a frontend that collects primary data points, which at this point is an Android app. This is the base CRUD and the starting point for a data point entering the ecosystem thus needs to be highly reliable

- **Data Analyses**: The external business need for generating insights from the collected data, This is about enabling as much as possible of the four layers of analytics within the platform -- **descriptive**, **diagnostic**, **predictive**, and **prescriptive**.

- **Integration**: Integration with 3rd Party APIs. For example, I was a client want all my data to show up on a Google sheet as they have other business workflows enabled from there.
 
 
### Challange
Creae Architectural solution for above requirments. Initially limit sope of this task to just descriptive analysis. <br/>
Some aspects of the solution to cover (as Frank McCourt once said, “the sky is the limit,” so feel free to not be limited to these): 
- Authorization levels in the platform
- What to use for and how to store the data points [schematics] coming in?
- Do you think we need multiple stores? If yes, streams vs. batch as a general data flow paradigm - use of one across the platform vs. a mix of things?
- Is moving data around really necessary? How do we mitigate the perils of such a setup?
- Keep resource usage [memory, CPU], throughput in mind
- How does all this get deployed?
- Already existing tools you’d want to use and what to build and why?
- How do you know this design will hold and up to when? is there a way to quantify/measure the quality of your design?
- Potential caveats in your solution
