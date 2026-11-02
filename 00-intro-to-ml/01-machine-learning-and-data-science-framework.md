# Scenario (KEIKO CORP - Hypothetical Organization)

- We need a Framework for our clients. Can you make one Please?!

### 1. Introducing our framework

_What we're going to cover (and what you'll finish with)_
_We're focused on..._

- Practical solution
- Writing machine learning code

_What ewe're going to cover_

**Steps in a full machine learning project**

1. Data Collection
2. Data Modeling\*
   - Problem definition: What problem are we trying to solve?
   - Data: What data do we have?
   - Evaluation: What defines success?
   - Features: What features should we model?
   - Modelling: What kind of model should we use?
   - Experiments: What have we tried/what else can we try?
3. Deployment

_\*Iterative process_

#### Steps

1. Create a framework
2. Match to data science and machine learning tools
3. Learn by doing

| Yes                | No                        |
| ------------------ | ------------------------- |
| Write code         | Overthink the process     |
| Make mistakes      | Try make things perfect   |
| Build projects     | Build things from scratch |
| Learn what matters |                           |

# [6 Step Machine Learning Framework](https://www.mrdbourke.com/a-6-step-field-guide-for-building-machine-learning-projects/)

1. Problem definition

- What problem was we trying to solve
- Supervised or Unsupervised or Classification or Regression

2. Data

- What kind of data do we have?
- Structured (Spreadsheets with rows and columns) or Unstructured (Image and audios)

3. Evaluation

- What defines success for us?
- House data => Machine learning model => House price => Predicted price and Actual price

4. Features

- What do we already know about the data?
- Heart disease? => Patient records => relationship between body weight and heart disease or other for pattern

5. Modelling

- Based on our problem and data, what model should we use?
- Problem 1 => Model 1
- Problem 2 => Model 2

6. Experimentation

- How could we improve/what can we try next?
- Attempt 1, 2, 3

# Types of Machine Learning Problems

- Problem definition: What problem was we trying to solve?

**When shouldn't you use machine learning?**

- Will a simple hand-coded instruction based system work?

**Main types of machine learning**

- Supervised Learning
- Unsupervised Learning
- Transfer Learning
- Reinforcement Learning

1. Supervised Learning:

- Data with Label
- Classification
  - "Is this example one thing or another"
  - Binary Classification = two options
  - Multi-class classification = more than two options
- Regression
  - How much will this house sell for?
  - How many people will buy this app?

2. Unsupervised learning

- Data with no label
- Clustering

3. Transfer Learning

4. Reinforcement Learning

**Matching your porblem**

- Supervised Learning: I know my inputs and outputs
- Unsupervised Learning: I am not sure of the outputs but I have inputs
- Transfer Learning: I think my problem may be similar to something else

# Types of Data

= What kind of data do we have

**Different types of data**

- Structured
- Unstructured

_Note:_

- Static: Which do not change over time
- The more data the better
- Streaming: Constantly change over time

_A data science workflow_
static data => jupyter => pandas => data analysis => matplotlib => machine learning models => heart disease

_What kind of data do you use?_

# Types of Evaluation

- What defines success for us?
- For this project to be worth pursuing further, we need a machine learning model with over 99% accuracy.

Table 1.0: Patient records => Machine Learning model => heart disease (Accuracy: 97.8%)

**Different types of metrics**

| Classification | Regression                     | Recommendation |
| -------------- | ------------------------------ | -------------- |
| Accuracy       | Mean absolute error (MAE)      | Precision at K |
| Precision      | Mean squared error (MSE)       |                |
| Recall         | Root mean squared error (RMSE) |                |

**Classifying car insurance claims**

Table 2.0" Car insurance claims => Machine Learning model (had to try a few of these) => Minimum accuarcy > 95%

**What do you measure?**

# Features in Data

- What do we already know about the data?

**Different features of data**

| ID   | Weight | Sex | Heart Rate | Chest Pain | Heart Disease |
| ---- | ------ | --- | ---------- | ---------- | ------------- |
| 4326 | 110kg  | M   | 81         | 4          | Yes           |
| 5681 | 64kg   | F   | 61         | 1          | No            |
| 7911 | 81 kg  | M   | 57         | 0          | No            |

_Table 1.0: Patient records_

- Feature variables: Weight, Sex, Heart Rate, Chest Pain
- target variable: Heart diseases

- Numerical feature: Weight, Heart Rate, Chest Pain
- Categorical features: Sex, Heart Disease
- Drived feature: Visit in last year (Categorical feature)

_Keynotes:_

- Feature enginerring: Looking at different features of data and creating new ones/altering existing one
- Feature coverage: Home many samples have different features? Ideally, every sample has the same features. Want > 10% coverage

_What are features of your problems?_

# Modeling - Splitting Data

- Based on our problem and data, what model should we use?

**3 parts to modelling**

- Choosing and training a model
- Tuning a model
- Model comparison

**The most important concept in machine learning (The training, validation and test sets or 3 sets)**

Split Your data

1. Training: Train your model on this
2. Validation: Tune your model on this
3. Test: Test and campare on this

Course materials (training set) => Practice exam (validation set) => Final exam (test set)

_keynotes_: Generalization: The ability for a machine learning model to perform well on data it hasn't seen before

**When things go wrong**
=> Practice exam (same as final exam set) => Final exam (already seen it)

Split 100 patient records

1. 70 patient records (training split 70-80%)
2. 15 Validation split(10-15%)
3. 15 Test split(10-15%)

_What was the last thing you testing your ability on?_

# Modelling - Picking the Model (Training Data)

- Based on our problem and data, what model should we use?

**Choose a model**

1. Problem 1 => Model 1
2. Problem 2 => Model 2

Structured Data
-> CatBoost, Dmlc XGBoost, Random Forest

Unstructured Data
-> Deep Learning, Neural network, Transfer Learning

**Training a Model**
Inputs and Outputs

X (data) => y (label)

**Goal: Minimise time between experiments**

| Experiment | Process                  | Accuracy | Training Time |
| ---------- | ------------------------ | -------- | ------------- |
| 1          | inputs, model 1, outputs | 87.5%    | 3 min         |
| 2          | inputs, model 2, outputs | 91.3%    | 92 min        |
| 3          | inputs, model 3, outputs | 94.7%    | 176 min       |

**Things to remember**

1. Some models work better than others on different problems
2. Dont be afraid to try things
3. Start small and build (add complexity) as you need

# Modelling - Tuning (Validation Data)

**Tuning a model**

- Cooking time: 1 hour, Temperature: 180C
- Cooling time: 1 hour, Temperature: 200C

Random forest => 3 trees => 5 trees

Neural Networks => 2 layers => 3 layers

**Things to remember**

1. Machine learning models have hyperparameters you can adjust
2. A models first results aren't its last
3. Tuning can take place on training or validation data sets

# Modelling - Comparison (Test Data)

- How will our model perform in the real world?

**Testing a model**

| Data Set | Performance |
| -------- | ----------- |
| Training | 98%         |
| Test     | 96%         |

**Underfitting (potential)**

| Data Set | Performance |
| -------- | ----------- |
| Training | 64%         |
| Test     | 47%         |

**Overfitting (potential)**

| Data Set | Performance |
| -------- | ----------- |
| Training | 93%         |
| Test     | 99%         |

**Overfitting and underfitting**

```
Before we get into the experimentation side of things, it's worth having a little reminder of overfitting and underfitting are.

All experiments should be conducted on different portions of your data.

Training data set — Use this set for model training, 70–80% of your data is the standard.

Validation/development data set — Use this set for model hyperparameter tuning and experimentation evaluation, 10–15% of your data is the standard.

Test data set — Use this set for model testing and comparison, 10–15% of your data is the standard.

These amounts can fluctuate slightly, depending on your problem and the data you have.

Poor performance on training data means the model hasn’t learned properly and is underfitting. Try a different model, improve the existing one through hyperparameter or collect more data.

Great performance on the training data but poor performance on test data means your model doesn’t generalize well. Your model may be overfitting the training data. Try using a simpler model or making sure your the test data is of the same style your model is training on.

Another form of overfitting can come in the form of better performance on test data than training data. This may mean your testing data is leaking into your training data (incorrect data splits) or you've spent too much time optimizing your model for the test set data. Ensure your training and test datasets are kept separate at all times and avoid optimizing a models performance on the test set (use the training and validation sets for model improvement).

Poor performance once deployed (in the real world) means there’s a difference in what you trained and tested your model on and what is actually happening. Ensure the data you're using during experimentation matches up with the data you're using in production.
```

1. Underfitting
2. Balanced (Goldilocks zone)
3. Overfitting

- Data leakage => Overfitting
- Data mismatch => Underfitting

_Fixes for overfitting and underfitting_

1. Underfitting:

- Try a more advanced model
- Increare model hyperparameters
- Reduce amount of features
- Train longer

2. Overfitting:

- Collect more data
- Try a less advanced model

**Comparing models**

| Experiment | Process                  | Accuracy | Training Time | Prediction time |
| ---------- | ------------------------ | -------- | ------------- | --------------- |
| 1          | inputs, model 1, outputs | 87.5%    | 3 min         | 0.5 sec         |
| 2          | inputs, model 2, outputs | 91.3%    | 92 min        | 1 sec           |
| 3          | inputs, model 3, outputs | 94.7%    | 176 min       | 4 sec           |

**Things to remember**

1. Want to avoid overfitting and underfitting (head towards generality)
2. Keep the test set separate at all costs
3. Compare apples to apples
4. One best performance metric does not equal best model
