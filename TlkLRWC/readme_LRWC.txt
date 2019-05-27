This file describes the data set LRWC available at https://research.yandex.com/datasets/toloka.

The data set is intended for non-commercial use. You must indicate that the data was obtained using Yandex.Toloka. If you plan to use the datasets for commercial purposes, obtain consent from Yandex by contacting: toloka@support.yandex.com. 

This dataset contains the opinions of Russian native speakers about the relationship between a generic term (hypernym) and a specific instance of it (hyponym). Assembled by Dmitry Ustalov in 2017. A set of 300 most frequent nouns was extracted from the Russian National Corpus. Then each method or resource (including RuThes and RuWordNet) produced at most five hypernyms, if possible. This resulted in 10,600 unique non-empty subsumption pairs, which were annotated by seven different performers whose mother tongue is Russian and were at least 20 years old as of February 1, 2017. As a result, 4,576 out of 10,600 pairs were annotated as positive while the remaining 6,024 were annotated as negative. Interestingly, the performers were more confident in the negative answers than in the positive ones.

Input data are in the file lrwc-1.1-assignments.tsv, the format is:
	<INPUT:hyponym>\t<INPUT:hypernym>\t<INPUT:genitive>\t<OUTPUT:judgement>\t<GOLDEN:judgement>\t<HINT:text>\t<ASSIGNMENT:link>\t<ASSIGNMENT:assignment_id>\t<ASSIGNMENT:worker_id>\t<ASSIGNMENT:status>\t<ASSIGNMENT:started>
Training tasks are in the file toloka-isa-50-skip-300-train-hit.tsv, the format is:
	<INPUT:hyponym>\t<INPUT:hypernym>\t<INPUT:genitive>\t<GOLDEN:judgement>\t<HINT:text>
Aggregated responses are in the file lrwc-1.1-aggregated.tsv, the format is:
	<INPUT:hyponym>\t<INPUT:hypernym>\t<INPUT:genitive>\t<OUTPUT:judgement>\t<CONFIDENCE:judgement>
	
Some statistics about the dataset are below.
	The number of main tasks: 74403. 
	The number of training tasks: 47.
	The number of aggregated assignments: 10600.