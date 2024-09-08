PA2_Altares, Raphael Carlos A.
1. Normalization Problem

        #Altares, Raphael Carlos A.
        #NORMALIZATION PROBLEM
        
        import numpy as np
        
        # make a 5x5 matrix with random numbers
        X = np.random.random((5, 5))
        print("Original Matrix:\n", X)  
        
        # find the mean and standard deviation of the matrix
        mean = X.mean()  
        std_dev = X.std() 
        
        # normalize the matrix (subtract mean and divide by standard deviation)
        X_normalized = (X - mean) / std_dev
        print("\nNormalized Matrix:\n", X_normalized)  
        
        # save the normalized matrix to a file called 'X_normalized.npy'
        np.save('X_normalized.npy', X_normalized)
        
        print("\nNormalization complete! The normalized matrix is saved as 'X_normalized.npy'.")
        
 2. Divisible by 3 Problem

        #Altares, Raphael Carlos
        #Divisible by 3 Problem
        
        import numpy as np
        
        # create a list of numbers from 1 to 100
        numbers = np.arange(1, 101)
        
        # square each number 
        squares = numbers**2
        
        # reshape the list into a 10x10 matrix
        A = squares.reshape(10, 10)
        
        # find elements in the matrix that are divisible by 3
        div_by_3 = A[A % 3 == 0]
        
        # save the result to a file named 'div_by_3.npy'
        np.save('div_by_3.npy', div_by_3)
        
        # print matrices for confirmation 
        print("10x10 Matrix of Squares:\n", A)
        print("\nElements Divisible by 3:\n", div_by_3)
        
        print("\nDone! The elements divisible by 3 are saved as 'div_by_3.npy'.")


          
                  
