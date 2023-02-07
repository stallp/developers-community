---
pagename: Overview
redirect_from:
  - data-engagement-history-overview.html
sitesection: Documents
categoryname: "Reporting"
documentname: Engagement History API
level-order: 6
order: 1
permalink: engagement-history-api-overview.html
root-link: true
indicator: chat
---
### Introduction

{: .attn-alert}
Our Data APIs enable you to retrieve many attributes and information types. Please refer to [API Data Metrics](https://developers.liveperson.com/api-data-metrics.html) for the different types of information and attributes which are retrievable via both [our Historical and Real Time Data APIs](overview.html).

Brands can now search, filter and keep copies of chat transcripts and related data, for example surveys, to later integrate and further analyze their data with third-party tools (DWH, CRM systems, etc.). 99.5 % of chat transcript data is available within 5 minutes. All other chat transcript data (including metadata like Engagement Attributes) is available within 2 hours after a chat has ended, and is stored for 13 months. The Engagement History API is based on the REST architecture style.

### Getting Started

A few things you'll need to get started with this API:

1. **Retrieve your domain**. Use the [LivePerson Domain API](agent-domain-domain-api.html) to retrieve this information by providing the following service name:

	* engHistDomain

2. This API requires authorization using API key.

	* **For a machine-to-machine authorizion using OAuth 1.0 App Keys OAuth 2.0 Client Credentials flow**
		* **OAuth 1.0 App Keys** — [follow the instructions](create-oauth-1-0-api-keys.html), to create and use an App key.

		{: .attn-note}
	For the Users API, select the Data category and check Conversation History / Messaging Interactions

		* **OAuth 2.0 Client Credentials flow** — [follow the instructions](oauth-2-0-client-credentials.html), to register an OAuth 2.0 application and generate a JWT access token **(Using version 2 of the Authorization API)**.

		{: .attn-note}
	When registering an OAuth 2.0 application for using the Engagement History API, use the “data.services.enghist” scope.


3. Note the [API terms of use](https://www.liveperson.com/policies/apitou).

### Use Cases

* Extract all chat transcripts and accompanying data in order to integrate with any 3rd party application or database

* Extract types of conversations (e.g. low CSAT score) and take an action on them.

View of Engagement History within Conversational Cloud:

![EngagementHistory](img/engagementhistory1.png)

Example of dashboard created using the API:

![EngagementHistory](img/engagementhistory2.png)
