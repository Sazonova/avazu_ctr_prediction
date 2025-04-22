I started by exploring a sample of the dataset, given its large size.
Before generating new features, I set aside the last day of the training data for validation, to avoid data leakage during the aggregation process.
I decided not to begin with Logistic Regression, as it felt too simplistic for this task. Instead, I built a LightGBM classifier and used Optuna for hyperparameter tuning.
I also checked paperswithcode.com for benchmarks and recent solutions. That’s where I got the idea to try a DeepFM model—and potentially, given more time, explore OptInter as a more recent alternative.
As expected, the dataset is highly imbalanced, so the models didn’t perform well on the first attempt. If I had more time, I’d dig deeper into the CTR topic to better understand which engineered features might help the model distinguish the target class more effectively.
I also ran PCA and t-SNE on the numerical features, but they didn’t show meaningful class separation.
Due to the initial poor model performance, I didn’t proceed with validation as planned, though it would have been part of the pipeline under better conditions.
Thank you for the interesting task—I’ve never worked with CTR data before, so it was a valuable learning experience.

