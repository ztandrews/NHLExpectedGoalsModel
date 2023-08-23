# Expected Goals Model
### Zach Andrews
### ztandrews18@sbcglobal.net
### github.com/ztandrews
---
#### About

##### This notebook houses the expected goals model creation code. I use my xG model for my [website]( https://statsbyzach-app.hf.space/home/), where I use the data to help understand the NHL in a smarter way. I'm uploading this notebook to GitHub on it's own to give everyone a clean, concise look at how the xG model was created, which can help provide a better understanding of the metrics I post on the site.

#### Why CatBoost?
##### I ended up going with the CatBoost Classifier because, along with giving me the best results out of other classifiers, it works very well with categorical data, of which there is a lot within my features. CatBoost is a very fast boosting algorithm, which made it an appealing choice and ultimately what I went with for the creation of the model.

#### The Data
##### The data I used to build this model with is sourced from the [Hockey-Scraper](https://github.com/HarryShomer/Hockey-Scraper) Python package, which I used to scrape every shot since 2010. Once I got the data, I extensively pre-processed it by feature engineering and cleaning up the data to prepare it for modeling. Note that the workbook to do this is not public yet, but I am actively working to make it a little cleaner so I can upload it.

#### Other Notes
##### Again, this notebook is just the creation of the model. Furthermore, I trimmed down the book a bit to make it easier to read and see how everything is working. I have a few separate books where I tested different algorithms, different features, and different evaluation methods, but this notebook only contains a clean version of the final model that I actually use. If you'd like to know more about how I reached a final decision on the features and algorithm of choice, feel free to reach out! Also, I have an automated process that applies the final model to every single shot taken in every NHL game that gets played in real time, which is how I add more data to my code base. 
