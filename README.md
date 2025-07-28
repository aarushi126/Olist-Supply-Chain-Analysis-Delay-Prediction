# Olist-Supply-Chain-Analysis-Delay-Prediction

As part of my exploration into supply chain analytics, I worked on a comprehensive data project using real-world datasets from Olist, one of Brazil’s largest e-commerce marketplaces. The goal of this project was to understand the key drivers of delivery delays, explore regional and product-level inefficiencies, and build a predictive model that can help the business proactively identify at-risk shipments.
The analysis began with merging and cleaning several datasets that covered customer orders, products, sellers, payments, delivery dates, freight values, and geolocation data. The first step was to get a consolidated view of Olist’s supply chain—how products move from sellers to customers across different regions of Brazil. During the cleaning process, I paid close attention to missing values, duplicates, empty strings, and inconsistent data types. This was essential to ensure the data was reliable enough to draw business insights from.

Once the data was prepared, I moved into an exploratory analysis phase. I focused on understanding patterns in delivery performance: which product categories experience the most delays, how freight charges relate to delivery time, and whether geography plays a role in logistics outcomes. I found that delays were especially common in the North and Northeast regions of Brazil—suggesting possible infrastructure or delivery route challenges. Certain product types like furniture and large electronics also had notably higher delay rates, likely due to bulkiness or special handling needs. Interestingly, I discovered that higher freight costs didn’t guarantee faster delivery, which opens up opportunities for Olist to optimize its logistics spending without compromising service.

To quantify and visualize these patterns, I built several KPIs and visual dashboards. These included average delivery times by state, freight efficiency scores, and delay percentages per product category. These visual insights could help Olist’s logistics and operations teams identify underperforming sellers, inefficient shipping routes, or categories that require extra care.
The most impactful part of the project was developing a predictive model to classify whether an order would be delayed or delivered on time. I engineered features based on order time (hour of day), freight cost, shipping distance (via geolocation), product price, and category. I trained both Logistic Regression and Random Forest models. While logistic regression performed well on accuracy due to class imbalance, it failed to correctly identify delayed orders. The Random Forest model, on the other hand, showed strong performance—especially in precision for delay prediction (91%), meaning when it flags a shipment as delayed, it’s usually correct. While the recall was moderate (14%), it’s still a useful model for business operations, acting as a reliable early-warning system that Olist could use to flag high-risk shipments and potentially intervene before a delay affects customer satisfaction.

Beyond model performance, I also pulled together a set of business insights that could guide Olist in improving its supply chain:

Product categories like furniture and seasonal décor are more likely to be delayed and need better planning.

Northern and Northeastern Brazil are hotspots for delays and may require targeted infrastructure improvements or new delivery partners.

Freight spending isn’t translating into faster delivery, which signals a potential inefficiency in how freight services are being selected.

Orders placed at night had a slightly higher probability of delays—perhaps due to warehouse processing cutoffs or next-day dispatching lags.

The Random Forest model can help reduce customer complaints and refund rates by proactively flagging risky orders.


Overall, this project demonstrates how data analytics and machine learning can transform complex logistical data into meaningful insights for a business. For a company like Olist, even small improvements in delivery performance can lead to better customer retention, reduced logistics costs, and smarter seller partnerships. If deployed in production, the model and insights developed here could help streamline Olist’s operations and elevate its delivery reliability across Brazil.
