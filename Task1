#' Author: Kayla Tabra
#' Date Created: 01/17/2024 
#' This R script demonstrates handling data in R, various data structures 
#' available, and demonstrate vector operations  

# Creating vectors ----
# Q1. Create a vector named numbers containing the integers from 1 to 20.
numbers <- seq(1L,20L,1L)

# Q2. Create a vector named names containing the following names: "Alice", "Bob", "Charlie", "David".
names <-c("Alice",  "Bob", "Charlie", "David")

# Q3. Create a vector named mixed_data containing the following values: 10, "hello", TRUE, 3.14.
mixed_data <-c(10, "hello", TRUE, 3.14)

# Q4. Access the third element of the names vector created in Q2. 
print(names)
names[3] #Index starts with 0

# Q5. Change the second element of the numbers vector created in Q1 to 50.
numbers[2] <-50
head(numbers)

# Creating Lists (Uses the objects created from questions Q1 to Q5) ----  
# Q6. Create a list named my_list containing the following elements: 
#       the vector numbers, the string "This is a list", and the logical value FALSE.
my_list <- list(numbers = numbers,
                  string = "This is a list", FALSE)
my_list

# Q7. Access the second element of the my_list list.
my_list[2]

# Q8. Add a new element to the my_list list: the character vector c("apple", "banana", "orange").
my_list$new_element <- c("apple","banana","orange")

# Creating Matrices ----  
# Q9. Create a 3x4 matrix named my_matrix with values ranging from 1 to 12, filled by row.
my_matrix <- matrix(seq(1, 12), nrow =3, ncol =4, byrow=TRUE)
my_matrix

# Q10. Create a 2x2 matrix named identity_matrix with 1s on the diagonal and 0s elsewhere.
identity_matrix <- matrix(seq(1,4), nrow = 2, ncol = 2)
diag(identity_matrix) <- 1
identify_matrix

# Q11. Extract the first row of the my_matrix matrix.
my_matrix[1, ]

# Q12. Calculate the transpose of the my_matrix matrix.
t(my_matrix)

# Creating Arrays ---- 
# Q13. Create a 3x4x2 array named my_array with random values between 0 and 100. 
#       Hint1: as.integer(runif(24, 0, 100)) --> Gives random 24 numbers between 0 and 100.
#       Hint2: sample(seq(0,100), 24) --> Also gives a sample of 24 numbers between 0 and 100.
# Generate 24 random integers between 0 and 100
array_input <- as.integer(runif(24, 0, 100)) 
array_input

my_array <- array(array_input, c(3,4,2))
my_array

# Q14. Access the element in the second row, third column, and first level of the my_array array.
my_array[2,3,1]

# Working with Factors ---- 
# Q15. Create a factor named gender with levels "Male" and "Female" and values c("Male", "Female", "Male", "Female").
gender <- factor(c("Male", "Female", "Male", "Female"), levels = c("Male", "Female"))
gender
a.integer(gender)

# Q16. Convert the character vector colors <- c("red", "blue", "red", "green") into a factor.
colors <- c("red", "blue", "red", "green")
colors

# Q17. Print the levels of the gender factor.
gender

# Creating Data frames. ---- 
# Q18. Create a data frame named students with columns "name", "age", and "grade", containing the following data:
#       name: c("Alice", "Bob", "Charlie")
#       age: c(18, 20, 19)
#       grade: c(95, 80, 90)
?data.frame()
my_list <- list(name = c("Alice", "Bob", "Charlie"),
                age = c(18, 20, 19),
                grade = c(95, 80, 90))
my_list$name
my_list$new_value <- c(50, 60)
my_list

students <- data.frame(name = c("Alice", "Bob", "Charlie"),
                       age = c(18, 20, 19),
                       grade = c(95, 80, 90))
students
students$new_value <- c(50,60,80)

# Q19. Access the "name" column of the students data frame.
students$name

# Q20. Add a new column named "city" to the students data frame, with values c("New York", "London", "Paris").
students$city <- c("New York", "London", "Paris")

# Q21. Select rows where the "grade" is greater than 90 in the students data frame.
students[1, ] # Fetch first row and all column values
students [1, c(2,3)] # Fetch only 2nd and 3rd columns 
students[c(1,2), c(2,3)] # Fetch only 2nd and 3rd columns for 1st or 2nd row
students[c(TRUE, TRUE, FALSE), c(2,3)] #Same as previous one. Fetch first 2 rows and 2nd and 3rd
students$grade > 90
students[students$grade > 90, ]
