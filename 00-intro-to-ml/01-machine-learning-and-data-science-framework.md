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
