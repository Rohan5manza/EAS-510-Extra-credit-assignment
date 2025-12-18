# EAS-510-Extra-credit-assignment
EAS 510 Basics of AI extra credit assignment, Inside Airbnb dataset 


Some Useful info: 

1. I downloaded listings.csv.gz and calendar.csv.gz for the mentioned cities and dates as needed. I uploaded them in respective separate folders in my Google Drive and mounted it to my colab instance, for easier management.
2. I used listings.csv.gz instead of simple listings.csv as there were additonal useful features in the former, which could give me more insights and hidden patterns for the models to uncover.
3. Make sure to run notebook with at least 12 GB RAM in Colab notebook instance ( easily avaiable via Colab Pro subscription), or else notebook may crash due to insufficient RAM, as processing huge data columns and performing havy operations like concat on them is RAM-heavy.
4. I personally loved this assignment as I learned a couple of new things, like how Xgboost can perform better than a neural network on classification, as it easily handles NaN values that neural networks cannot. Gemini tells me this is because : " XGBoost uses a technique called Sparsity-aware Split Finding. When it encounters a missing value, it actually learns which direction (left or right branch of the tree) is the best "default" path for missing data. It’s very smart and doesn't crash. Neural Networks, being purely mathematical functions (linear algebra), simply cannot handle "undefined" values. ". I found this fact interesting.
5. I also learned that additional scaling was needed before I could train neural network, so I log-scaled the values so outliers cannot influence my model a lot. Outliers being that some Airbnbs were priced a lot ( like $1000 ) , compared to others. 
