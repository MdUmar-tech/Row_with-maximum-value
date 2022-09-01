# Row_with-maximum-value
Print specific rows with highest value from multiple columns using R Studio
#DATAFRAME
dput(dta)
structure(list(A = c(45, 20, 9, 6, 6), B = c(23, 34, 7, 10, 5
), C = c(12, 15, 8, 0, 4), D = c(4, 4, 6, 0, 3), E = c(5, 6, 
3, 1, 2)), class = "data.frame", row.names = c("BOX_A", "BOX_B", 
"BOX_C", "BOX_D", "BOX_E"))

###Now find which column is the maximum:
idx <- apply(dta, 1, which.max)

######
###Now display the rows where the maximum is in the first column. This is not what you asked for but it is what your picture shows:

dta[idx==1, ]
#        A  B  C D E
# BOX_A 45 23 12 4 5
# BOX_C  9  7  8 6 3
# BOX_E  6  5  4 3 2
