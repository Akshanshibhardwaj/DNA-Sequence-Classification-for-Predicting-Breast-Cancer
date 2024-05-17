# DNA-Sequence-Classification-for-Predicting-Breast-Cancer


### What is the problem?
### What is a possible approach to solve this problem?
### What is the final precision?

# DNA Sequence Classification for Predicting Breast Cancer

> This project provides the classification of DNA sequences for Breast cancer prediction which into promoter regions associated. Using machine learning and deep learning techniques, I analyze and try to predict sequence data for negative and positive answers in cancer prediction. The goal is to improve understanding of gene regulation in cancer and possible treatment approaches.

> Promoter sequences are critical points for regulation elements in the genome that control gene expression, moreover, this approach could help us to understand how to recognize cancers faster or recognize them in early stages. Identifying these regions accurately can provide insights into genetic controls involved in breast cancer. This project employs various machine learning algorithms to classify sequences as promoter-positive or promoter-negative based on their nucleotide composition.

> In this project, it will show the Machine Learning Model for classifying DNA sequences. K-Nearest Neighborhood and Support Vector Machine and several algorithms to find out wich algorithm can have the best precision for our problems.



#  Model Performance Analysis:

> 1. **K Nearest Neighbors & Gaussian Process**


*   Accuracy: Both models registered an accuracy of 85.19%.

*   Precision and Recall: Showcased exemplary precision in identifying non-promoter sequences (class 0), albeit with a diminished recall, suggesting some true negatives were overlooked. Conversely, their detection of promoter sequences (class 1) was highly effective, marked by flawless recall tempered by marginally reduced precision.

*   Analysis: The prominent recall for class 1 underlines the models' efficacy in contexts where the cost of missing a promoter sequence exceeds the inconvenience of false positives.

---

> 2. **Decision Tree:**


*   Accuracy: Marginally lower at 81.48%.
*   Balance: Exhibits a well-maintained balance between precision and recall across classes, resulting in a fair but unspectacular performance per class.

*   Utility: This model is well-suited for applications that require a balanced approach to sensitivity and specificity but falls short in scenarios demanding high precision.

---


> 3. **Random Forest:**


*   Accuracy: This model underperformed with a 70.37% accuracy.

*   Issues: Demonstrated notably lower precision and recall for non-promoter sequences, indicating potential overfitting or inability to generalize effectively from training data.

*   Considerations: Enhancements in parameter tuning and expanding the training dataset could potentially uplift its performance, suggesting its latent capacity to pre-emptively identify possible cancers.

---


> 4. **Neural Network & AdaBoost:**


*   Accuracy: Impressively high at 92.59%.

*   Strengths: Both models demonstrated robust precision and recall, ensuring reliable performance across both classes.

*  Recommended Use: Optimal for critical applications where minimizing classification errors is paramount.

---


> 5. **Naive Bayes:**


*   Accuracy: A solid performance with an accuracy of 88.89%.

*   Characteristics: Maintains a decent equilibrium between precision and recall, with a slight preference for precision in non-promoter sequences.

*  Application: Particularly effective in initial screenings where fast and reasonably accurate classifications are critical.

---


> 6. **SVM (Support Vector Machine) Variants:**


1.   Linear & RBF Kernels:

*   Accuracy: Stellar at 96.30%.
*   Performance: Both kernels were proficient, with the RBF kernel achieving perfect recall for class 0 and high precision for class 1.

*   Optimal Choice: These models are recommended for their exceptional ability to manage linearly inseparable data.


2.   Sigmoid Kernel:

*   Accuracy: Slightly lower at 88.89% compared to other SVM kernels.

*  Detail: Showed less consistency in precision and recall across classes than its SVM counterparts.

*   Usage: Best used in situations where data exhibits a non-linear distribution, albeit less effectively than the RBF kernel.




#### conclusion:

> These outcomes have indicated that machine learning models can have different results because of data characteristics in breast cancer research.  High-recall models such as Neural Networks and AdaBoost are valuable in clinical settings where missing a diagnosis has severe consequences. However, SVM models with an RBF kernel are perfect for providing high precision and recall. Also, they could be necessary for reliable predictions. This analysis has shown the significance of model application in improving Diagnostic accuracy and, by extension, patient outcomes in oncology.





### In this project we saw a comprehensive approach to optimize the hyperparameters of an SVM model using Particle Swarm Optimization (PSO). Initially, a function was defined to evaluate the model's performance using multiple metrics, providing a detailed assessment of its strengths and weaknesses. Subsequently, the PSO algorithm was utilized to find the optimal hyperparameters (C and tol) that minimized the mean squared error. The optimized SVM model demonstrated improved precision, highlighting the effectiveness of the optimization process in enhancing model performance. This approach underscores the value of advanced optimization techniques in achieving robust and reliable machine learning models.

