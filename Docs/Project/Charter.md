# Project Charter

## Business background

* Santander
* Fraud detection in the customers

## Scope
* What data science solutions are we trying to build?
* Deep learning models to determine the fraudulent client
* Train a neuronal model to classify the customer activities. To determine if they are fraudulent.
* Proceed all the bank's clients data every 2 weeks to determine if there are any fraudulent action.

## Personnel
* Who are on this project:
	* KK:
		* Project lead: 1
		* PM: 1
		* Data scientist(s): 4
		* Account manager: 1
	* Santander:
		* Data administrator: 2
		* Business contact: 2
	
## Metrics
* What are the qualitative objectives? (e.g. reduce user churn)
* Indentification of fraudulent activities.
* What is a quantifiable metric  (e.g. reduce the fraction of users with 4-week inactivity)
* Improving the recall to the 95% in the detection.
* Quantify what improvement in the values of the metrics are useful for the customer scenario (e.g. reduce the  fraction of users with 4-week inactivity by 20%)
* Improving the recall by 30% 
* What is the baseline (current) value of the metric? (e.g. current fraction of users with 4-week inactivity = 60%)
* Current frau detectio recall = 65%
* How will we measure the metric? (e.g. A/B test on a specified subset for a specified period; or comparison of performance after implementation to baseline)
* We will measure and compare the recall of both model respect the dataset is given.
## Plan
* Phases (milestones), timeline, short description of what we'll do in each phase.

## Architecture
* Data
  * What data do we expect? Raw data in the customer data sources (e.g. on-prem files, SQL, on-prem Hadoop etc.)
* Data movement from on-prem to Azure using ADF or other data movement tools (Azcopy, EventHub etc.) to move either
  * all the data, 
  * after some pre-aggregation on-prem,
  * Sampled data enough for modeling 

* What tools and data storage/analytics resources will be used in the solution e.g.,
  * ASA for stream aggregation
  * HDI/Hive/R/Python for feature construction, aggregation and sampling
  * AzureML for modeling and web service operationalization
* How will the score or operationalized web service(s) (RRS and/or BES) be consumed in the business workflow of the customer? If applicable, write down pseudo code for the APIs of the web service calls.
  * How will the customer use the model results to make decisions
  * Data movement pipeline in production
  * Make a 1 slide diagram showing the end to end data flow and decision architecture
    * If there is a substantial change in the customer's business workflow, make a before/after diagram showing the data flow.

## Communication
* How will we keep in touch? Weekly meetings?
* Who are the contact persons on both sides?
