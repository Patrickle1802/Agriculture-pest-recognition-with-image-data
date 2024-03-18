# Agriculture-pest-recognition-with-image-data

**Problem Definition:**
The project involves developing and evaluating machine learning models for pest detection in agricultural settings, using a dataset containing 2,479 real images of five different types of agricultural pests: Ants, Bees, Grasshoppers, Moths, and Wasps.

The objective of this project is to enhance pest recognition models for effective deployment in practical agricultural environments.

**Proposed Approaches:**
- Two deep learning models with different architectures utilizing Convolutional Neural Networks (CNN) techniques are created and compared for classifying these pest images.
- Key experiments focus on hyperparameter tuning (filters, dense layers, kernel size), image quality, optimizer selection (RMSprop, Adam, Adadelta), loss function (categorical_crossentropy, huber), and other model configurations.

**Major Findings:**
1. Parameter Optimization:
The optimization process involved a meticulous exploration of model parameters to enhance pest detection in agricultural settings. Key findings shed light on the pivotal choices in model configuration. Notably, experiments demonstrated that increasing the number of filters beyond 32 did not substantially improve performance but risked overfitting. A kernel size of (1,1) emerged as a favorable choice, allowing the model to capture fine-grained patterns in the data. Additionally, it was observed that a smaller image size of (50,50,3) effectively balanced computational efficiency with the capacity to capture relevant features. The dense layer with 200 units displayed suitability for extracting high-level abstractions, although further fine-tuning may offer optimization opportunities. Furthermore, a dropout rate of 0.25 struck an optimal balance between regularization and model capacity. The selection of the categorical cross-entropy loss function and the RMSprop optimizer, with specific hyperparameter settings, contributed to model stability during training. Overall, these parameter optimization findings informed the development of a robust model for pest detection.

2. Model performance
Across all the experiments Model 1 (with above mentioned parameters) outperforms all others, achieving the highest accuracy (64%), substantial agreement (Kappa coefficient of 0.552), and a balanced F1-Score of 0.64. This indicates that Model 1 correctly classifies a significant portion of test samples while maintaining a good trade-off between minimizing false positives and false negatives.

3. Improving pest recognition models for agriculture is an ongoing process that requires a combination of data, technology, and domain knowledge, in accordance with following potential approaches:
- Data Quality: Collect diverse and representative data encompassing various crops, growth stages, lighting conditions, and pests for a robust model foundation.
- Accurate Labels: Ensure precise pest labeling to maximize model training effectiveness.
- Data Augmentation: Apply techniques like rotation, scaling, cropping, and flipping to expand the training dataset, reducing overfitting risks.
- Preprocessing: Employ noise reduction and image enhancement (contrast, brightness, sharpness adjustments) to improve image quality.
- Class Balance: Address class imbalances by oversampling minority classes or using focal loss to enhance detection of challenging pests.
- Continuous Learning: Implement systems for ongoing data updates to adapt to evolving pest populations and environmental changes.
- Iterative Improvement: Continually evaluate model performance in real-world agricultural scenarios and refine models based on feedback and emerging data trends.
