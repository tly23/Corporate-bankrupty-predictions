# Corporate-bankrupty-predictions
# Team-119
 Team 119's group project GitHub repository for MGT 6203 (Canvas) Spring of 2024 semester.

## Steps to Run:

- Ensure R and RStudio are installed.
- Clone the repo to your local machine.
- Install R packages specified in requirements.txt.
- Make sure you're on the "main" branch if there are other branches.
- Locate the .Rmd "bankruptcy-logit-knn.Rmd" in the Code folder.
- Run the .Rmd file (Run All).
- It should locate the root directory and find the appropriate folders, etc. using the "here" package.

## Code Process

```mermaid
  graph TD;
      A["Conduct summary stats"]-->B;
      B["Define the financial ratio (FR) groups"]-->C;
      C["Calculate correlation matrices on FR Groups"]-->D;
      D["Run Principal Component Analysis on each FR group"]-->E;
      E["Plot the principal components"]-->F;
      F["Get top # components & top # variables by absolute loadings"]-->G;
      F-->K["Identify top components using charts"]
      K-->G
      G["Train and test logistic regression models on FR subsets"]-->H;
      H["Plot logit model accuracies"]-->I;
      I["Train and test KNN models on FR subsets"]-->J;
      J["Plot KNN model accuracies"]-->L["Done!"];
```
