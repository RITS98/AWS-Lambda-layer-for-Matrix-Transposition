# AWS-Lambda-layer-for-Matrix-Transposition

This assignment focuses on the creation of a Python function capable of transposing a 2-dimensional matrix of numbers, packaging this function as a reusable AWS Lambda Layer, and then utilizing this layer in a separate AWS Lambda function. This task will demonstrate the reusability of code in cloud environments, specifically within AWS, and introduce the concept of Lambda Layers as a means to share code, libraries, and other dependencies across multiple Lambda functions.

## Steps:

1. Python Code
   ```
    def transpose(matrix):
      """
      Transposes the given matrix.
  
      Parameters:
      matrix (list of list of int/float): The matrix to transpose
  
      Returns:
      list of list of int/float: The transposed matrix
      """
      # Using list comprehension to transpose the matrix
      transposed_matrix = [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
      
      return transposed_matrix
   ```

2. Creating the layer
   ![image](https://github.com/RITS98/AWS-Lambda-layer-for-Matrix-Transposition/assets/51791113/76458ea8-73a1-4eb7-9005-e0e18a24c37f)

3. Add the layer in the Lambda function
   ![image](https://github.com/RITS98/AWS-Lambda-layer-for-Matrix-Transposition/assets/51791113/3e3a467c-724d-42d3-8fb6-13d5a5c6136c)

4. Test Result
   
   ![image](https://github.com/RITS98/AWS-Lambda-layer-for-Matrix-Transposition/assets/51791113/8985a234-190f-4201-a657-1721c69e6732)
   ![image](https://github.com/RITS98/AWS-Lambda-layer-for-Matrix-Transposition/assets/51791113/4fbf9ec6-cb1e-4f81-b25f-cfe68a259a51)

