Good day,
I’m writing regarding the first task of our course, “Data Analysis.” Myself and Anastasiya Alekseeva want to form a team for all tasks. We want to use the “Horse Survival Dataset” (source: https://www.kaggle.com/datasets/yasserh/horse-survival-dataset) that describes horse medical record (features) and what eventually happens to it (target/classes). We chose this dataset as it’s a relatively small dataset with many features to choose from, which seems ideal for the task. However, we decided to remove some features to more closely follow guidelines and eliminate features with many missing values. Here are the features that were selected (left in the dataset):
* surgery - whether a horse had surgery or not (categorical: yes or no)
* age - age of a horse (categorical: adult or young)
* pulse - heart rate in beats per minute (integer)
* respiratory_rate - number of breaths taken per minute (integer)
* capillary_refill_time - time taken for color to return to an external capillary bed after pressure is applied to cause blanching (categorical: less_3_sec or more_3_sec)
* abdominal_distention - indicates gut motility, highlighted as important (categorical: none, slight, moderate, severe)
* packed_cell_volume - number of red cells by volume in the blood (integer)
* total_protein - dataset description only mentions that it inversely correlates with dehydration; we suspect that it represents the total amount of protein in the blood (float)
 
The target class will be a column “outcome” that shows what happened to the horse (categorical: lived, died, was euthanized).
There are also repeating visits, indicated by “hospital_number.” We use this column to remove duplicates and keep the first element as we want to predict a horse's future on the first try.
The resulting dataset has 8 features with 1 target (9 columns) with 165 examples (rows).
