library(readxl)
library(forecast)
# Read the data from Excel into R
#exercise1.xlsx is not available here, but has data
mydata <- read_excel("exercise1.xlsx")

# Look at the first few lines of mydata
head(mydata)

# A tibble: 6 x 4
# ``     Sales AdBudget   GDP
# <chr>  <dbl>    <dbl> <dbl>
# 1   Mar-81  1020      659   252
# 2   Jun-81   889      589   291
# 3   Sep-81   795      512   291
# 4   Dec-81  1004      614   292
# 5   Mar-82  1058      647   279
# 6   Jun-82   944      602   254


# Create a ts object called myts
# ts(data, start, frequency, ...)
myts <- ts(mydata[,2:4], start = c(1981, 1), frequency = 4)

################################## Execise 2

# Plot the data with facetting
autoplot(myts, facets = TRUE)

# Plot the data without facetting
autoplot(myts, facets= FALSE)

# Plot the three series
autoplot(gold)
autoplot(woolyrnq)
autoplot(gas)


# Find the outlier in the gold series
goldoutlier <- which.max(gold)

# Look at the seasonal frequencies of the three series
frequency(gold)
frequency(woolyrnq)
frequency(gas)

