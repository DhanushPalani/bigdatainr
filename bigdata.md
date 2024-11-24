# Ex.No:6. Implement an application that stores big data in R
## Aim
To implement a big data storage application using R.

## Procedure

1.Install R and required packages (RSQLite, data.table).
2.Use a large dataset to demonstrate data storage and retrieval.
## Code/Steps
```
# Load library
library(data.table)

# Generate big data
big_data <- data.table(ID = 1:1000000, Value = rnorm(1000000))

# Save to disk
fwrite(big_data, "big_data.csv")

# Load back into memory
big_data_loaded <- fread("big_data.csv")
print(head(big_data_loaded))
```
## Result
Successfully demonstrated big data storage and retrieval using R.

