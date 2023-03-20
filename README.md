# Business_Model
**PROBLEM STATEMENT**

Consumer sentiment is a crucial factor that businesses need to consider in order to thrive in today's competitive market. Understanding how consumers feel about their products and services can help companies tailor their marketing strategies to better target their audience and improve their sales.

To this end, we are developing a predictive machine learning model that will analyze social media activity to determine consumer sentiment towards various types of content. The model will consider a range of features in the social media data, including the latest news, popularity on social media platforms, and the topic of media resources.

This project is of utmost importance for businesses as it provides an opportunity to obtain valuable insights into consumer sentiment, which can be used to inform decision-making and ultimately drive success. By accurately predicting consumer reactions to different types of content, companies can tailor their messaging and advertising to appeal to their target audience, potentially leading to increased customer engagement and sales.

**TASK IN HAND**

As of 2023, there has been an increasing trend in social media usage, with billions of users engaging with various types of content such as text, images, and videos. With the rise of social media, businesses have also started leveraging these platforms to engage with their customers and promote their products and services.

To analyze the sentiments of consumers towards different types of content, machine learning models have been developed using various libraries in Python, such as Scikit-learn, TensorFlow, and Keras. In addition to these, the use of the Intel One API library has also gained popularity, as it provides a unified programming model for accelerating data analytics and machine learning workloads across multiple architectures, including CPUs, GPUs, and FPGAs.

To optimize the machine learning models, various techniques such as hyperparameter tuning, feature selection, and data preprocessing have been used. With the increasing amount of social media data available, these models have become more complex and require efficient optimization techniques to provide accurate predictions.

Overall, the development of machine learning models to predict consumer sentiment towards different types of content based on social media activity has become increasingly important in the current digital age, and the use of various libraries and optimization techniques has helped improve the accuracy and efficiency of these models.

**LIBRARIES**


Pandas is a versatile and user-friendly open-source tool for analyzing and manipulating data quickly and efficiently.

Numpy is a crucial building block for scientific Python and PyData ecosystems, providing an extensive set of functions for numerical computing.

The "re" module offers functions that enable you to determine whether a specific string matches a given regular expression.

The Natural Language Toolkit (NLTK) is a powerful platform that allows developers to create Python applications for working with human language data.

Word Cloud is a data visualization technique that represents text data in a visually appealing way, where the size of each word corresponds to its frequency or importance within the given data set.

**1. Data Cleaning**


1. convert the title and heading into lowercase
2. removing the punctuations
3. removing unnecessary emojis
4. removing stop words 
5. remove punctuation from the text
6. lemmatization using Spacy so that we can count the appearance of each word. Lemmatization removes the grammar tense and transforms each word into its original form.

**2.Model Building**


To build a sentiment analysis model, the preprocessed data needs to be converted into a format that can be used as input for the model.
 The feature extractor used is the chi-squared test (chi2) with the SelectKBest method from the scikit-learn library. The SelectKBest method is used to select the top k features that are most relevant to the output variable.
 The preprocessed training dataset needs to be split into training and validation datasets, with the training dataset used to train the model, while the validation dataset is used to evaluate the model's performance and tune hyperparameters. The model which we have selected is made using logistic regression. The chosen model is trained on the preprocessed training dataset, which allows it to predict the sentiment of a given text input.
 The trained model is evaluated on the preprocessed testing dataset, and if its performance is unsatisfactory, additional preprocessing steps or feature extraction methods can be tried, or different models or hyperparameters can be experimented with. 
Once the model's performance is satisfactory, it can be deployed to predict the sentiment of new text inputs.

**Intel® Extension for Scikit-learn***


Patching scikit-learn with the Intel Extension for Scikit-learn involves replacing the original scikit-learn algorithms with their optimized counterparts provided by the extension. This patching can be undone, allowing users to revert to the original scikit-learn implementation if needed.
Different patching methods are available to support different scenarios of enabling the extension, all of which achieve the same optimized result. These patching methods are interchangeable and can be used based on the user's preference or requirements.
Overall, patching scikit-learn with the Intel Extension for Scikit-learn allows users to take advantage of the optimized versions of the algorithms provided by the extension, resulting in faster and more efficient data analysis and machine learning tasks.

**Improving and deploying the model**


If the performance of the model is not meeting the desired standards, additional preprocessing steps or feature extraction methods can be explored. Alternatively, experimenting with different models or hyperparameters can also be considered to enhance the model's performance. In the current model, logistic regression was utilized, which resulted in an accuracy of 78%.
Once the model's performance meets the expected level, it can be deployed to predict the sentiment of new text inputs. Further improvements can be made by including additional independent variables, such as engagements corresponding to Google Plus, LinkedIn, and Facebook, to enhance the model's accuracy.
While testing of the model is still pending, the satisfactory results obtained from the training process and dataset splitting are encouraging.
