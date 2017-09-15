### Assignment 4
The goal of this assignment is to evaluate the impact of compensation for injuries at work on injury duration. Look at the variable description by using the following code to get their exact definition. 

```sh
library(foreign) 
myData=read.dta("e:/INJURY.dta") 
var.labels <- attr(myData,"var.labels") 
data.frame(var.name=names(myData),var.labels) 
```

Q1. What is the expected effect of compensation on the injury duration? Can we do a simple regression of the compensation on the duration? Why or why not? 

Q2. Explain that there could be different responses for low-earners or high-earners.  

Q3. Regress the log of duration (durat) on a dummy indicating whether the observation is before or after the change in benefits (afchnge), a dummy indicating whether the individual is a high earner or not (highearn), and the interaction of both (afchnge*highearn). Interpret the results.  
 
Q4. How could omitted variables affect the estimation? Include the control variables that seem adequate in your regression model. Try to justify why we need those variables. Compare the results of the model with control variables and the model without control variables. 

Q5. Explain the potential problem of the above model. 
