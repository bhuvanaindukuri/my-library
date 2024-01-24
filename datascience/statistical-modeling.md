### Statistical modeling

#### Basics
- Types of Variables
  - Response variables
    - Outcome, target or dependent variables
    - Variables that you seek to predict
  - Predictor variables
    - input, explanatory or independent variables
    - Used to predict the value of response variables
- Variable values can be
  - Continuous
    - Numerical value
  - Categorical
    - Non numeric values Ex: On, off
  - Ordinal
    - Similar to categorical but have a heirarchy Ex: low, medium, high
- Types of Models
  - General linear model
  - logistic regression
- Logic for choosing the models

```mermaid
  flowchart TD
    A[Choose Model] -->|Response Variable| B(Value Type)
    B --> C{Value Type}
    C -->|Continuous| D1(Error Type) 
         D1 --> D2{Distribution}
         D2 --> |Normal| D3[General Linear model]
         D3 --> D4[Y=b0+b1x1+b2x2....+bkxk+e]
    C -->|Continuous| E1(Predictor Variable) 
         E1 --> E2{Types}
         E2 --> |Categorical| E3[ANOVA]
         E2 --> |Continuous| E4[Least squares regression]
    C -->|Categorical & Binary| F1[Logistic Regression] 
         F1 --> F2["logit(Y) = b0+b1x1+b2x2....+bkxk"]
```
  
