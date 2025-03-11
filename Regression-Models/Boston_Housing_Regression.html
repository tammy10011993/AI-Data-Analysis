---
title: "House Price Prediction using Multiple Regression"
author: "Your Name"
date: "`r Sys.Date()`"
output: html_document
---

# 📊 Introduction
# This project applies Multiple Linear Regression (OLS) to predict house prices using the Boston Housing Dataset.
# Various factors such as crime rate, number of rooms, and tax rates are analyzed to understand their impact on house prices.

```{r}
# Load necessary libraries
library(MASS)
library(ggplot2)
library(caTools)
```

# 🔹 Load Dataset
```{r}
# Load Boston housing dataset
data("Boston")
head(Boston)  # View first few rows
```

# 🔹 Exploratory Data Analysis (EDA)
```{r}
# Summary statistics
summary(Boston)

# Correlation matrix
cor(Boston)

# Plot relationship between crime rate & house price
ggplot(Boston, aes(x = crim, y = medv)) +
  geom_point(color = "blue") +
  labs(title = "Crime Rate vs House Price", x = "Crime Rate", y = "Median House Price")
```

# 🔹 Train-Test Split
```{r}
set.seed(100)
split <- sample.split(Boston$medv, SplitRatio = 0.65)
train <- subset(Boston, split == TRUE)
test <- subset(Boston, split == FALSE)
```

# 🔹 Build Linear Regression Model with Two Variables
```{r}
# Fit the multiple linear regression model with two variables
Reg1 <- lm(medv ~ lstat + rm, data = train)

# Model summary
summary(Reg1)
```

# 🔹 Build Linear Regression Model with All Variables
```{r}
# Fit the multiple linear regression model using all independent variables
Reg2 <- lm(medv ~ ., data = train)

# Model summary
summary(Reg2)
```

# 🔹 Identify Significant Variables and Improve Model
```{r}
# Checking p-value significance to identify important variables
significant_vars <- summary(Reg2)$coefficients[,4] < 0.05
important_features <- names(which(significant_vars))
print("Significant Variables:")
print(important_features)

# Ensure that Intercept is removed from the list
important_features <- setdiff(important_features, "(Intercept)")

# Rebuilding the model with only significant variables
formula <- as.formula(paste("medv ~", paste(important_features, collapse = " + ")))
RefinedReg <- lm(formula, data = train)

# Model summary after feature selection
summary(RefinedReg)
```

# 🔹 Model Evaluation
```{r}
# Predict on test data
predictions_Reg1 <- predict(Reg1, newdata = test)
predictions_Reg2 <- predict(Reg2, newdata = test)
predictions_Refined <- predict(RefinedReg, newdata = test)

# Calculate R-Squared for all models
SSE_Reg1 <- sum((test$medv - predictions_Reg1)^2)  # Sum of Squared Errors
SST <- sum((test$medv - mean(test$medv))^2)  # Total Sum of Squares
R_squared_Reg1 <- 1 - (SSE_Reg1/SST)

SSE_Reg2 <- sum((test$medv - predictions_Reg2)^2)
R_squared_Reg2 <- 1 - (SSE_Reg2/SST)

SSE_Refined <- sum((test$medv - predictions_Refined)^2)
R_squared_Refined <- 1 - (SSE_Refined/SST)

R_squared_Reg1
R_squared_Reg2
R_squared_Refined
```

# 🔹 Final Line Plots of Fitted vs Actual Values
```{r}
library(ggplot2)

# Create dataframe for plotting
train_results <- data.frame(
  Actual = train$medv,
  Fitted_Reg1 = fitted(Reg1),
  Fitted_Reg2 = fitted(Reg2),
  Fitted_Refined = fitted(RefinedReg)
)

# Convert data to long format for ggplot
library(reshape2)
melted_results <- melt(train_results, id.vars = "Actual", variable.name = "Model", value.name = "Fitted")

# Plot Fitted vs Actual for all models
ggplot(melted_results, aes(x = Actual, y = Fitted, color = Model)) +
  geom_line() +
  geom_abline(slope = 1, intercept = 0, linetype = "dashed", color = "black") +
  labs(title = "Fitted vs Actual - Comparison of Models", x = "Actual Values", y = "Fitted Values") +
  theme_minimal()
```

# 🔹 Conclusion
```{r}
# The model with two variables, the model with all variables, and the refined model are compared.
# R-squared values indicate how well each model explains price variation.
# The refined model, using only significant variables, may offer better interpretability and performance.
```

# 🔹 Export Notebook
```{r}
# Save notebook as an HTML report
rmarkdown::render("Boston_Housing_Regression.rmd")

library("rmarkdown")
rmarkdown::convert_ipynb("Boston_Housing_Regression.rmd")
