This file describes the data set TlkAgg2 available at https://research.yandex.com/datasets/toloka.

The data set is intended for non-commercial use. You must indicate that the data was obtained using Yandex.Toloka. If you plan to use the datasets for commercial purposes, obtain consent from Yandex by contacting: toloka@support.yandex.com. 

The task was to assess the relevance of a document for a query as 0 or 1. The main metric of quality is accuracy of aggregated labels estimated as the fraction of the aggregated labels equal to the golden labels over the golden set. Workers identification, tasks information and labels names were anonymized.

Accuracy results for some aggregation models are:
	Majority Vote: 77.21%
	Dawid Skene: 81.3%
	GLAD: 78.34%

Crowdsourced labels are in the file crowd_labels.tsv, the format is:
	<worker-id>\t<task-id>\t<label>
Golden labels are in the file golden_labels.tsv, the format is:
	<task-id>\t<label>

Some statistics about the dataset are below.
	The number of crowdsourced labels: 475536.
	The number of tasks labelled by crowdsourced workers: 99319; 
 		mean workers per task: 4.79, standard deviation: 0.69; 
 		median workers per task: 5.0. 
	The number of workers performing the tasks: 7138; 
 		mean tasks per worker: 66.62, standard deviation: 85.44; 
 		median tasks per worker: 40.0. 
	The distribution of classes in crowdsourced labels:
		1: 0.58;
		0: 0.42.
	The number of tasks with golden labels: 10079.
	The distribution of classes in golden labels:
		0: 0.6
		1: 0.4
	Accuracy of workers:
		mean: 63.29%
		median: 66.67%
	Average accuracy of crowdsourced labels: 69.94%
