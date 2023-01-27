
# a simple calculator 
# opertors are +,-,/,* 
# in the string form 
# ny numbers will be in int 
# user interface should ask user three things ,
# 1). Num1 (int )
# 2). Num2 (int)
# 3). the operation  (str))
# print the result on the basis of the selection 
val = 'y'

while(val!='n'):
    Num1 = int(input('Enter the Num1 : '))
    Num2 = int(input('Enter the Num2 : '))
    # have a concept of a flag 
    
    flag = 0
    while(flag==0):
        op = input('Enter the Operation: ')
        Result = 0 # initializing the result 
        if(op=='+'):
            Result = Num1 + Num2
            print('The Addition of ',Num1,' and ',Num2,' is ',Result)
            flag=1
            
        elif(op=='-'):
            Result = Num1 - Num2
            print('The Subtraction of ',Num1,' and ',Num2,' is ',Result)
            flag=1
        elif(op=='/'):
            Result = Num1 / Num2
            print('The division of ',Num1,' and ',Num2,' is ',Result)
            flag=1
        elif(op=='*'):
            Result = Num1 * Num2
            print('The Multiplication of ',Num1,' and ',Num2,' is ',Result)
            flag=1
        else:
            print('Invalid Operator Selected ')
            flag=0
            print('Please Re enter the Correct option (+,-,/*)')
    # completion of the whole operation 
    val = input('Do you want to Continue??? (y/n): ')

print('end of the code ')
