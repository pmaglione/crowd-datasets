This file describes the data set TlkAgg5 available at https://research.yandex.com/datasets/toloka.

The data set is intended for non-commercial use. You must indicate that the data was obtained using Yandex.Toloka. If you plan to use the datasets for commercial purposes, obtain consent from Yandex by contacting: toloka@support.yandex.com. 

The task was to assess the relevance of a document for a query on a 5-graded scale. Some tasks in this data set have more than one golden label, in such cases all the golden labels are considered equally correct. The main metric of quality is accuracy of aggregated labels estimated as the fraction of the aggregated labels equal to one of the golden labels for a given task from the golden set.
Additionally to the crowdsourced labels there is information about workers that were banned for a certain reason. For each banned worker the reason for banning is provided as one out of four ban types, details about each ban type are not given. Workers identification, tasks information and labels names were anonymized.

Accuracy results for some aggregation models are:
	Majority Vote: 89.92%
	Dawid Skene: 90.72%
	GLAD: 90.16%

Crowdsourced labels are in the file crowd_labels.tsv, the format is:
	<worker-id>\t<task-id>\t<label>
Golden labels are in the file golden_labels.tsv, the format is:
	<task-id>\t<label>
Bans for workers are in the file bans.tsv, the format is:
	<worker-id>\t<ban-reason>

Some statistics about the dataset are below.
	The number of crowdsourced labels: 1091918
	The number of tasks labelled by crowdsourced workers: 363814;
 		mean workers per task: 3.0 , standard deviation: 0.75;
 		median workers per task: 3.0.
	The number of workers performing the tasks: 1273;
 		mean tasks per worker: 857.75, standard deviation: 1684.48;
 		median tasks per worker: 198.0.
	The distribution of classes in crowdsourced labels:
		1: 0.05;
		2: 0.01;
		3: 0.36;
		4: 0.18;
		5: 0.39.
	The number of tasks with golden labels: 33860;
 		mean labels per task: 1.36, standard deviation: 0.48;
 		median labels per task: 1.0;
	The distribution of classes in golden set:
		1: 0.12;
		2: 0.27;
		3: 0.27;
		4: 0.16;
		5: 0.19.
	Accuracy of workers:
		mean: 77.11%;
		median: 82.63%.
	Average accuracy of crowdsourced labels: 84.3%.
	The number of banned workers: 90
