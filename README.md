# Choice-Based Conjoint Analysis for “PopFlicks” a Streaming Service:

**Built with Python in Jupiter Notebook**

**Python Libraries Used: "Pandas, Numpy, Matplotlib, Statsmodel, and Squarify"**

## Summary:

Choice-Based Conjoint (CBC) Analysis is a popular form of conjoint analysis used to identify how a respondent values combinations of features. It's based on the principle that any product or service can be broken down into a set of attributes that ultimately impact users' perceived value of an item or service.

In a CBC analysis, respondents are presented with a series of choices that represent potential products or services. Each choice is composed of a combination of different attributes and levels, such as price, color, size, or other product-specific features. Respondents are then asked to choose their most preferred option from each set of choices.

The data collected from these choices is used to calculate numerical values called "preference scores" or "part-worth utilities". These scores indicate how much each attribute and level influenced the respondent's choices. These preference scores can then be used to simulate market scenarios and predict consumer behavior.

PopFlicks has shared their CBC customer survey data, which contains customer opinions on various product features. These features include but are not limited to: increasing new content (e.g., Disney and HBO), expanding the number of accounts, offering different price levels, and assessing the frequency of ads. PopFlicks is seeking an analysis of this data to gain insights on potential product improvements based on customer feedback.

In this project we document our observations as we explore, build, and compare using Logistic Regression.

We initiate the data preparation process by isolating the dependent and independent variables from the survey dataset. Next, we perform transformations on the independent variables to create their corresponding dummy variables. Following this, we establish a Logistic Regression model to obtain part-worth values. These part-worth values are subsequently organized into a data frame and visualized through a horizontal bar graph.

Next, our focus shifts to analyzing specific drivers, and we create separate subplots for each category of features. Subsequently, we compile a dictionary containing the coefficients of all features to determine their importance. This is achieved by calculating the difference between the maximum and minimum coefficient values for each feature. We then compute the total importance value and use it to calculate the relative importance of each feature. This information is used to construct a data frame, which we then visualize using a treemap.

Later, PopFlicks expressed interest in exploring the possibility of incorporating additional content alongside advertisements. To delve into this inquiry, we initiated our analysis by generating an interaction term between extra content and ads using the customer data. We then constructed a model and conducted logistic regression to derive the part-worth values associated with this interaction. Finally, leveraging these values, we crafted a subplot illustrating the results of introducing extra content with ads at the same time.
