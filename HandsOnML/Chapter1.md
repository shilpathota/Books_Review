
# Chapter 1: The Machine Learning Landscape - Questions & Answers
## 1.How would you define Machine Learning?


**Answer:** Machine Learning is about building systems that can learn from data.
## 2.Can you name four types of problems where it shines?


**Answer:** Machine Learning shines in problems such as:<br/>
- Automatically classifying news articles.
- Automatically flagging offensive comments.
- Summarizing long documents.
- Creating a chatbot or personal assistant.
- Making your app react to voice commands (speech recognition).
- Detecting credit card fraud (anomaly detection).
- Segmenting clients based on their purchases (clustering).
- Representing a complex dataset in a clear diagram (data visualization, often using dimensionality reduction).
## 3. What is a labeled training set?
**Answer:** A labeled training set is a set of data instances where each instance comes with the expected output, or label. For example, in the California housing dataset, each instance (district) includes the median housing price, which is the label.
## 4. What are the two most common supervised tasks?
**Answer:** The sources mention classification and regression as common supervised learning tasks.
## 5. Can you name four common unsupervised tasks?
**Answer:** Common unsupervised tasks include:
- Clustering.
- Anomaly detection.
- Density estimation.
- Mixture models.
- Dimensionality reduction.
## 6. What type of Machine Learning algorithm would you use to allow a robot to walk in various unknown terrains?
**Answer:** The task of creating agents capable of taking actions in an environment to maximize rewards over time is associated with Reinforcement Learning.
## 7. What type of algorithm would you use to segment your customers into multiple groups?
**Answer:** Clustering algorithms are used to segment clients into multiple groups based on their purchases.
## 8. Would you frame the problem of spam detection as a supervised learning problem or an unsupervised learning problem?
**Answer:** Spam detection is framed as a supervised learning problem because the system learns from labeled examples of spam and ham emails.
## 9. What is an online learning system?
**Answer:** An online learning system can learn incrementally as new data arrives. This is in contrast to batch learning, where the system is trained once using all available data.
## 10. What is out-of-core learning?
**Answer:** The provided text mentions out-of-core learning as a type of batch learning used when the dataset is too large to fit in memory, requiring the data to be processed in chunks.
## 11. What type of learning algorithm relies on a similarity measure to make predictions?
**Answer:** The source mentions Instance-based learning algorithms.
## 12. What is the difference between a model parameter and a learning algorithm’s hyperparameter?
**Answer:** Model parameters are values learned by the algorithm during training, while hyperparameters are parameters of the learning algorithm itself, set before training, and control the learning process.
## 13. What do model-based learning algorithms search for? What is the most common strategy they use to succeed? How do they make predictions?
**Answer:** Model-based learning algorithms search for the model parameter values that minimize a cost function. Once trained, they make predictions by feeding new instances to the learned model.
## 14. Can you name four of the main challenges in Machine Learning?
**Answer:** The sources state that Chapter 1 discusses challenges, but a specific list of four main challenges is not detailed in the provided excerpts.
## 15. If your model performs great on the training data but generalizes poorly to new instances, what is happening? Can you name three possible solutions?
**Answer:** This indicates overfitting. While the source mentions that tuning hyperparameters on the test set can lead to poor generalization, specific solutions are not listed as answers to this question in the provided text of Chapter 1.
## 16.What is a test set, and why would you want to use it?
**Answer:** A test set is a subset of data, typically 20% or less, held back from training. You use a test set to evaluate the final model's performance on new instances to estimate how well it will generalize.
## 17. What is the purpose of a validation set?
**Answer:** The purpose of a validation set is to compare different models and fine-tune hyperparameters to select the best model and hyperparameters before evaluating on the test set.
## 18. What is the train-dev set, when do you need it, and how do you use it?
**Answer:** The provided sources do not explicitly mention a "train-dev set" by this name. The text discusses training, validation, and test sets.
## 19. What can go wrong if you tune hyperparameters using the test set?
**Answer:** If you tune hyperparameters using the test set, the model will perform great on the test set but generalize poorly to new instances.
