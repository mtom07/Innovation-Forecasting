# Swire Innovation Product Forecasting
This repository showcases individual and group work completed to address a business problem presented to our MSBA Capstone Group at the University of Utah.

# Business Problem and Project Goal
Swire Coca-Cola is a leader in the beverage distribution industry based out of Salt Lake City. Swire distributes many different beverages across regions in the western half the of the United States. In their product portfolio they often do short term releases of “Innovation” products. These products are crucial for maintaining customer interest, driving demand, and staying ahead of the competition, but they also pose risks of overproduction or underestimating demand. We are tasked with creating a method to accurately forecast demand of 7 upcoming innovation products, that will be distributed in various regions and for various amounts of time.

# Our Group Solution
In examining and working with the provided historical data our team was able to create a method for forecasting each of the 7 products as well as any further upcoming products. Our solution created a process that consist of 4 steps. Step 1 is to create an “innovation” data set. This data set is created by finding items like our innovation products in brand, flavor, packaging size, and product category. Once the innovation data set was created step 2 was to use linear regression to assure the similar items selected were helpful in model creation. Step 3 was to one hot encode our remaining features to create an XGboost model that will provide prediction for our items. Step 4 was to do a comparison check against the brands previous innovation launches and the innovation launces of our previous products. This last step assured that our recommended predictions matched real world result. With this process in place, we created a forecast for each of the new 7 products as well as gave a tiered recommendations on which products we believe would do best.

# Business Value
With the implementation of this new model, Swire will effectively utilize their historical data to forecast any innovation product. The process will enable quick and efficient comparison of the performance of new products with data from previous innovations. Additionally, the models will provide insights into the confidence levels for production quantities. This will assist in making crucial decisions, firstly determining whether to proceed with a product launch, and subsequently understanding the optimal production volume and timing for each innovation product, while also estimating the margin of error in the forecast.

# My Contribution
Our project approach was divided into three sections: EDA, Modeling, and Final Predictions. In each section, every group member had specific tasks to accomplish. During the EDA section, I was tasked with comparing each of our seven innovation products to the overall dataset, identifying comparison products for each, and conducting analysis on when innovation products had historically sold best. In the Modeling stage, I focused on two of the seven products, creating a dedicated innovation dataset for each. Subsequently, I ensured that the features in the dataset were applicable to my products and developed an XGBoost model for each. During the Final Predictions step, I provided predictions for each product, determined an optimal launch period for each, and made recommendations on if the product should go to production. For one product, an energy drink, I confidently predicted units and time due to numerous historical comparisons leading to high model performance. However, for the second product, although I created predictions for units and a launch period, I ultimately did not recommend launching it due to low model performance, primarily stemming from limited historical data.

# Difficulties
Throughout the process, we encountered several challenges, with the first being the size of the dataset. We were tasked with analyzing a dataset containing millions of rows, resulting in prolonged processing times and significant noise during modeling. Additionally, we struggled to accurately predict future performance. To address this, we explored various modeling techniques including ARIMA, Random Forest, Linear Regression, and XGBoost. While we achieved success in training and testing these models, we faced discrepancies when applying them to our innovation products, as the predictions did not align with real-world historical scenarios.

# Learnings
Although this process presented significant challenges, it also offered many new learning opportunities. Throughout the project, I was able to improve my knowledge in working with large datasets and utilizing tools like Tableau for exploratory data analysis (EDA). I expanded my skills in R, learning new techniques for manipulating extensive datasets, such as employing loops for efficient data engineering and visualizing and segmenting data effectively. In the modeling phase, I deepened my understanding of feature selection, one-hot encoding, and tuning XGBoost models to achieve accurate results. However, the most crucial lesson learned was the importance of validating our modeling results against real-world scenarios. While our initial model performance metrics were high, they did not align with practical outcomes. Conducting this reality check enabled us to refine our data preparation processes and develop models that gave us accurate forecasts.
