# Deep Learning Lab 2 - Neural Networks and Backpropagation

This repository contains the implementation and analysis for Deep Learning Lab 2, focusing on neural network architectures, backpropagation understanding, and hyperparameter tuning.

## 📋 Lab Overview

This lab explores fundamental concepts in deep learning through hands-on experiments with:
- Backpropagation algorithm understanding
- Neural network architecture design
- Hidden layer size optimization
- MNIST digit classification with MLPs
- Regularization techniques (L1/L2)
- Performance visualization and analysis

## 🗂️ Repository Structure

```
Deep-Learning-Lab2/
├── README.md                          # This file
├── Backprop_modified.ipynb           # Exercise 1: Backpropagation Analysis
├── NN_sample_modified.ipynb          # Exercise 2: Hidden Layer Size Study
├── answers_exercise2.txt             # Exercise 2: Analysis and Answers
├── MNIST_MLP_improved.ipynb          # Exercise 3: MNIST Classification with Improvements
└── [registration_number].txt         # Repository link file
```

## 🚀 Exercises and Results

### Exercise 1: Backpropagation Understanding
**File:** `Backprop_modified.ipynb`

**Objective:** Analyze how the number of training epochs affects model accuracy.

**Key Modifications:**
- Increased training iterations from default to higher values
- Observed convergence behavior and accuracy improvements
- Documented the relationship between training time and performance

**Results:**
- Training with more epochs generally improved accuracy
- Demonstrated diminishing returns after optimal epoch count
- Identified potential overfitting with excessive training

### Exercise 2: Hidden Layer Size Analysis
**File:** `NN_sample_modified.ipynb`

**Objective:** Study the impact of hidden layer size on neural network performance.

**Experiment Setup:**
- Tested hidden layer sizes: [1, 2, 3, 4, 5, 20, 50]
- Used planar dataset for binary classification
- 5000 training iterations per configuration

**Key Results:**
| Hidden Units | Accuracy |
|--------------|----------|
| 1            | 67.50%   |
| 2            | 67.25%   |
| 3            | 91.00%   |
| 4            | 90.75%   |
| 5            | 91.50%   |
| 20           | 91.25%   |
| 50           | 90.25%   |

**Key Findings:**
- **Critical threshold effect**: Dramatic improvement from 2→3 hidden units (67% → 91%)
- **Optimal performance**: 5 hidden units achieved best accuracy (91.50%)
- **Overfitting signs**: Slight performance decline with excessive nodes (50 units)
- **Bias-variance tradeoff**: Clear demonstration of underfitting → optimal → overfitting transition

### Exercise 3: MNIST MLP with Improvements
**File:** `MNIST_MLP_improved.ipynb`

**Objective:** Improve MNIST digit classification through hyperparameter tuning and regularization.

**Improvements Implemented:**

#### A. Hyperparameter Tuning
- Experimented with different learning rates, hidden units, and dropout rates
- Tested multiple architectures for optimal performance
- Systematic comparison of configurations

#### B. Regularization
- **L1 Regularization**: Added L1 penalty to prevent overfitting
- **L2 Regularization**: Implemented weight decay for better generalization
- Combined L1+L2 regularization for enhanced performance

#### C. Performance Analysis
- **Confusion Matrix**: Class-wise performance visualization
- **Training Curves**: Accuracy and loss progression analysis
- **Class-wise Accuracy**: Individual digit recognition performance

**Results:**
- Achieved improved test accuracy through systematic optimization
- Regularization helped reduce overfitting
- Comprehensive performance analysis with visual insights

## 🔧 Technical Implementation

### Dependencies
- Python 3.x
- TensorFlow/Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Running the Code
All notebooks are designed to run in Google Colab:

1. Upload the notebook to Google Colab
2. Upload required supporting files (planar_utils.py, testCases.py, etc.)
3. Install dependencies if needed:
   ```python
   !pip install tensorflow numpy matplotlib seaborn scikit-learn
   ```
4. Execute cells in order

## 📊 Key Insights and Learning

### Neural Network Architecture Design
- **Model Complexity**: Balance between underfitting and overfitting
- **Hidden Layer Sizing**: Critical threshold effects in capacity
- **Regularization Impact**: L1/L2 penalties improve generalization

### Optimization Strategies
- **Hyperparameter Tuning**: Systematic approach yields better results
- **Training Monitoring**: Early stopping and validation curves
- **Performance Metrics**: Multiple evaluation approaches for comprehensive analysis

### Theoretical Understanding
- **Bias-Variance Tradeoff**: Practical demonstration through experiments
- **Capacity Control**: How model complexity affects learning
- **Regularization Theory**: Preventing overfitting through constraints

## 📈 Results Summary

### Best Performing Configurations
- **Exercise 2**: 5 hidden units → 91.50% accuracy
- **Exercise 3**: Regularized MLP → [Your best accuracy]% on MNIST

### Key Performance Metrics
- Training accuracy progression
- Validation performance monitoring
- Test set generalization results
- Class-wise classification performance

## 🎯 Conclusions

This lab successfully demonstrated:

1. **Architecture Importance**: Proper hidden layer sizing is crucial for performance
2. **Training Dynamics**: Understanding convergence and optimization behavior  
3. **Regularization Benefits**: L1/L2 penalties improve generalization
4. **Systematic Analysis**: Data-driven approach to hyperparameter optimization

The experiments provided practical insights into neural network design principles and validated theoretical concepts through hands-on implementation.

## 👤 Author

**Registration Number:** IT22165770  
**Course:** Deep Learning  
**Lab:** Lab 2 - Neural Networks and Backpropagation

## 📝 Notes

- All experiments conducted in Google Colab environment
- Results may vary slightly due to random initialization
- Notebooks include detailed markdown documentation
- Supporting files required for complete execution

---

*This repository demonstrates practical application of neural network concepts and provides comprehensive analysis of key deep learning principles.*
