
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

- ## Showing decimal places 
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

- ## For showing histogram
  <pre>
   w = -6 + sqrt(10)*(randn(1,100000))
   hist(w)
  </pre>
- ## For showing N bars in histogram in above scenerio
  <pre>
   hist(w,N)
  </pre>

- ## For showing identity matrix
  <pre>
   eye(3)
  </pre>

- ## For knowing details about any function
  <pre>
    help function_name
    help randn
  </pre>