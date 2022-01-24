
- ## How to clear a octave terminal
  <pre>clc
  </pre>
- ## For comment we use % operator
  <pre>
  a = ( 1 == 0) %false
  </pre>
- ## For Not equal operation we use ~= 
  <pre>
   a = (1 ~= 0) %true
  </pre>

- ## XOR operation between two numbers
  <pre>
   xor(1,0)
  </pre>

- ## For printing a variable don't use semicolon . Use semicolon if you don't want to print 
  
  <pre>
   a = pi ; %it will print nothing
   a = pi   %it will print value of pi
  </pre>

- ## Another way of displaying variable
  <pre>
  disp(a) %it will print value of pi 
  </pre>

- ## displaying decimal places 
  <pre>
   disp(sprintf('4 decimal places : 0.4f',a)) %it will print value of pi upto 4 decimal places
  </pre>

- ## Creating a Matrix 

  <pre>
   A = [ 1 2 ; 3 4 ; 5 6 ]
   A = [ 1 2 
        3 4
        5 6 ]
  </pre>

- ## Creatng a vector 
  <pre>
  A = [ 1 ; 2 ; 3]
  A = [
       1 
       2
       3
      ]
  </pre>

- ## Creating a 1 X N dimensional matrix which value wil start with A and end with B by increasing D at a time
 
  <pre>
  v = A : D : B
  v = 1 : 0.5 : 3 

  v = [ 1 1.5 2 2.5 3]
  </pre>

- ## Creating a 1 X N dimensional matrix which value wil start with A and end with B by increasing 1 at a time
  
  <pre>
  v = A : B 
  v = 1 : 6 
  v = [ 1 2 3 4 5 6]

  </pre>

- ## Creating  a A X B dimensional matrix all filled with one or zero

  <pre>
   v = ones(A,B)
   v = ones(2,3)
   v =  [
           1 1 1
           1 1 1 
        ]
   
   x = zeroes(A,B)
   x = zeroes(1,3)
   x = [
        0 0 0
       ]
  </pre>
- ## Creating  a A X B dimensional matrix all filled with random value

  <pre>
   v = rand(A,B)
  </pre>

- ## Creating  a A X B dimensional matrix all filled with negative random value

   <pre>
    v = randn(A,B)
   </pre>

- ## For displaying histogram
  <pre>
   w = -6 + sqrt(10)*(randn(1,100000))
   hist(w)
  </pre>`

- ## For displaying N bars in histogram in above scenerio
  <pre>
   hist(w,N)
  </pre>

- ## For displaying identity matrix
  <pre>
   eye(3)
  </pre>

- ## For knowing details about any function
  <pre>
    help function_name
    help randn
  </pre>

- ## For knowing dimension of a matrix A 
  <pre>
   size(A)
  </pr e>
- ## For knowing 1st dimension of a matrix A 
  <pre>
   size(A,1)
  </pre>
- ## For knowing 2nd dimension of a matrix A 
  <pre>
   size(A,2)
  </pre>
- ## For knowing largest dimension of a matrix . It is mainly used for vectors .
   <pre>
   length(A) 
   length([1;2;3;4;5]) %this will return 5 . which is the row number of this vector 
   </pre>

- ## For knowing Current directory
  <pre>pwd
  </pre>
- ## Going to a directory
  <pre> cd 'path'
  </pre>
- ## Displaying all the files in a path
  <pre>ls
  </pre>
- ## For loading a file
  <pre>
  load filename
  load('filename')
  </pre>
- ## For knowing which variables are used 
   <pre>who</pre>
- ## For knowing which variables are used with additional information
   <pre>whos</pre>
- ## For clearing memory
   <pre> clear </pre>
- ## For clearing a certain variable
   <pre> clear variable_name </pre>
- ## Saving a vector called 'v' in a file called 'filename' in binary format
   <pre> save filename v</pre>
- ## Saving a vector called 'v' in a file called 'filename' in human readable format 
   <pre> save filename v -ascii </pre>

- ## For displaying a element of jth column in ith row
   <pre>A(i,j)</pre>
- ## For displaying all the elements of ith row
   <pre>A(i,:)</pre>
- ## For displaying all the elements of jth column
   <pre>A(:,j)
- ## For displaying specific rows of a matrix 
   <pre> 
   A([i j k], :)
   A([1 3 4], ;)  % it will display 1st,2nd and 4th row of matrix
   </pre>
- ## Replacing a column of a M X N matrix by another vector of M X 1 vector
  <pre>
  A = [
     1 2 3 
     4 5 6
     7 8 9
  ]
  A(:,2) = [10 ; 11 ; 12]
  A = [
    1 10 3 
    4 11 6 
    7 12 9
  ]
  </pre>
- ## Replacing a row of a M X N matrix by another vector of 1 X N matrix
  <pre>
    A = [
    1 10 3 
    4 11 6 
    7 12 9
  ]
  A(3,:) = [21 22 23]
  A = [
    1 10 3 
    4 11 6 
    21 22 23
  ]
  </pre>
- ## Appending N X 1 vector as a column to M X N matrix
  <pre>  A = [
    1 10 3
    4 11 6
    21 22 23
   ]
   A = [A,[41 ; 42 ; 43]]
   A = [
    1 10 3 41
    4 11 6 42
    21 22 23 43
   ]
  </pre>

- ## Putting All elements in a single column vector
  <pre>
   A = [
     1 2 
     3 4
     5 6
   ]
   A(:)
   A = [
     1
     3
     5
     2
     4
     6
   ]
  </pre>
 - ## Suppose A is a matrix of M X N dimension and B is a matrix of M X P dimension now by adding two matrix and create a M X (N+P) dimensional matrix
  <pre>
  A = [ 
    1 2 
    3 4
  ]
  B = [
    5 6 7 8
    9 10 11 12
  ]
   
  C = [A B]

  C = [
    1 2 5 6 7 8
    3 4 9 10 11 12
  ]

  </pre>

- ## Suppose A is a Matrix of M X N dimension and B is a matrix of P X N dimension now by adding two matrix and create a (M + P) X N dimensional matrix
  <pre>
  A = [
    1 2
    3 4
    5 6
  ]
  B = [
    7 8
    9 10
    11 12
    13 14
  ]
  C = [ A ; B]
  C = [
    1 2
    3 4
    5 6
    7 8
    9 10
    11 12
    13 14
  ]

  </pre>

- ## Suppose A matrix is M X N dimensional and B Matrix is N X P dimensional the the result matrix will be M X P dimensional 
  <pre>
   A = [
     1 2 
     3 4
     5 6 
   ]
   B = [
     7 8 9
     10 11 12
   ]
   C = A * B
  </pre>

- ## We can also do element wise matrix operations .
  <pre>
   A = [
     1 2
     3 4
   ]
   B = [
     5 6
     7 8
   ]
   C = A .* B
   C = [
     5 12
     21 32
   ]
   
  D = 1 ./ A
  D = [
    1 0.5 
    0.33 0.25
  ]
  E = exp(A)
  E = [
    1.7183 7.3891
    20.0855 54.5982
  ]
  </pre>

- ## How to Transpose a matrix of M X N to N X M matrix
  <pre>
  A = [
    1 2 
    3 4
    5 6
  ]
  B = A'
  B = [
    1 3 5
    2 4 6
  ]

  </pre>

- ## How to find the highest value and index of an element from a M X 1 dimensional matrix or 1 * N dimensional matrix
  <pre>
  A = [ 7 ; 11 ; 13 ; 2]
  [val,ind] = max(A)
  val = [ 13 ] 
  ind = [ 3 ]
  B = [ 10 19 17 15]
  [val,ind] = max(B)
  val = [ 19 ] 
  ind = [2]
  </pre>

- ## For A = M X N dimensional matrix where M > 1 and N > 1 max(A) will return max value of every column and row number of the max element of every column . 
  <pre>
   A = [
     6 9
     13 5
   ]

   [val,ind] = max(A)
   val = [13 9]
   ind = [2 1]
  </pre>

- ## For A = 1 X N dimensional matrix find(A >= val) will return the column number of the elements which has value >= val . For B = M X 1 dimensional matrix find(B >= val) will return the row number of the elements which has value >= val .For the First case will be  1 X P dimensional matrix where P is the number of elements which follows above condition and for the second case it will be P X 1 dimensional matrix(vector)
  <pre>
   A = [ 1 5 7 9];
   ind = find( A >= 5 )
   ind = [2 3 4]
   B = [ 9 ; 11 ; 2 ; 1]
   ind = find ( B <= 2)
   ind = [ 
           3 
           4
         ]
  </pre>
  
- ## For C = M X N dimensional matrix where M > 1 and N > 1 find(C >= val ) will return two P X 1 dimensional matrices(vectors) . One is for the row indexes of the element which follows above condition and other is for the column indexes of the corresponding element . Here P is the number of element which follows above condition 

  <pre>
  A = [ 1 2 11 ; 3 13 15 ; 17 4 19]
  [r,c] = find (A <= 4)

  r = [
    1
       2
       1
       3
  ]

    c = [
       1
       1
       2
       2
     ]
  </pre>

- ## For any M X 1 or 1 X N dimensional matrix sum,prod these function will return a single value . But for any M X N dimensional matrix where M > 1 and N > 1 there sum,prod these functions will return sum for every column thus a 1 X N dimensional matrix

  <pre>
  A = [ 1 2 3 4]
  ans = sum(A)
  ans = 10
  B = [ 1 2 3 4]
  ans = sum(B)
  ans = 24
  C = [
      1 2 3 
      4 5 6
  ]
  ans = sum(C)
  ans = [5 7 9]
  </pre>

- ## ceil,floor this functions works for any value of M and N in any M X N dimensional matrix

  <pre>
  A = [
    1.67 2.33 3.01
    2.33 6.666 7.00
  ]
   
  ans = ceil(A)

  ans = [
     2 3 4
     3 7 7
  ]
  </pre>

- ## for any A = M X N dimensional matrix max(A,[],1) and max(A) is same . it returns the max value of each column and create a 1 X N dimensional matrix
  <pre>
  A = [ 2 3 4 ; 3 7 7]
  ans = max(A,[],1)
  ans = [ 3 7 7]
  </pre>

- ## for any A = M X N dimensional matrix max(A,[],2)  returns the max value of each row and create a M X 1 dimensional matrix

  <pre>
  A = [ 2 3 4 ; 3 7 7]
  ans = max(A,[],2)
  ans = [ 
         4 
         7
        ]
  </pre>

- ## How to take the max element of a A = M X N matrix rather than taking max element rowwise/columnwise ? There is two way to do this . One is max(max(A)) and other one is max(A(:))
  <pre>
  A = [
    1 2 3 
    4 5 6
    1 2 3
  ]
  ans = max(max(A))
  ans = [6]
  ans = max(A(:))
  ans = [6]
  </pre>

- ## How to inverse a matix A 
  <pre>
  pinv(A)
  </pre>