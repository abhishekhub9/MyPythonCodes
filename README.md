# MyPythonCodes
***************************| 1. Palindrome Check | ************************************
test_number= input ("Enter the number :" )
print ("The original number is : " + str(test_number))

# using str() + string slicing
# for checking a number is palindrome
res= str(test_number)[::-1]
res1 = str(test_number) == res

print ("is the number palindrome? :" +str(res1))

if (res1==True):
    print("And the reverse number is same as orignal one :" + str(res))
    
else:
    print("Sorry! Reverse number is different than original :" +str(res))
    
---
OUTPUT- 1:
Enter the number :121
The original number is : 121
is the number palindrome? :True
And the reverse number is same as orignal one :121

OUTPUT- 2:
Enter the number :3261
The original number is : 3261
is the number palindrome? :False
Sorry! Reverse number is different than original :1623
-----------------------------------------------------------------------------------

*************************| 2. Factors of a Number |***********************************
def print_factors(x):
    ##This function tales a number and print it's factors
    print("The factors of",x,"are:")
    for i in range (1,x+1):
        if x % i ==0:
            print (i)
num=int(input("Enter the number:"))

print_factors(num)
        
---
OUTPUT:
Enter the number:2019
The factors of 2019 are:
1
3
673
2019
----------------------------------------------------------------------------------------

*******************************|3(a). Fibonacci Series Without Recursion|******************
##user Input
nterms= int(input("How many terms? "))

##First two terms
n1 = 0
n2 = 1
count = 0

##check if the number of terms is valid
if nterms <= 0:
    print("Negative numbers are not part of fibonacci series")
elif nterms == 1:
    print("Fibonacci sequence upto",nterms,":")
    print(n1)
else:
    print("Fibonacci sequence upto",nterms,":")
    while count < nterms:
        print(n1,end=' , ')
        nth=n1+n2
        ##update values
        n1 =n2
        n2 = nth
        count +=1
---
OUTPUT:
How many terms? 25
Fibonacci sequence upto 25 :
0 , 1 , 1 , 2 , 3 , 5 , 8 , 13 , 21 , 34 , 55 , 89 , 144 , 233 , 377 , 610 , 987 , 1597 , 2584 , 4181 , 6765 , 10946 , 17711 , 28657 , 46368 ,
--------------------------------------------------------------------------------------------------------------------
