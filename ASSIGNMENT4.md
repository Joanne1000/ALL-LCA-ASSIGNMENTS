Input:
# Create two matrices using nested lists 
matrix1 = [
    [1, 2, 3],
    [4, 5, 6]
]
matrix2 = [
    [7, 8, 9],
    [10, 11, 12]
]

# Initialize a result matrix with the same size
result = [
    [0, 0, 0],
    [0, 0, 0]

]

# Perform matrix addition
for i in range(len(matrix1)):         # loop through rows
    for j in range(len(matrix1[0])):  # Loop through columns
         result[i][j] = matrix1[i][j] + matrix2[i][j]

# Display the result
print("Matrix 1:")
for row in matrix1:
    print(row)

print("\nMatrix 2 :")
for row in matrix2:
    print(row)

print("\Sum of Matrix 1 and Matrix 2:")
for row in result:
    print(row)

Output:
Matrix 1:
[1, 2, 3]
[4, 5, 6]

Matrix 2 :
[7, 8, 9]
[10, 11, 12]
\Sum of Matrix 1 and Matrix 2:
[8, 10, 12]
[14, 16, 18]
