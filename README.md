# class-vs-instance
class Person:
    def __init__(self,initialAge):
        if initialAge<0:
            print('Age is not valid, setting age to 0.')
            self.age=0
        else:
            self.age=initialAge
    def amIOld(self):
        if self.age<13:
            print('You are young.')
        elif self.age < 18:
            print('You are a teenager.')
        else:
            print('You are old.')
    def yearPasses(self):
        self.age+=1
        

t = int(input())
for i in range(0, t):
    age = int(input())         
    p = Person(age)  
    p.amIOld()
    for j in range(0, 3):
        p.yearPasses()       
    p.amIOld()
    print("")
    
    output:
    Input (stdin)

4
-1
10
16
18
Expected Output

Age is not valid, setting age to 0.
You are young.
You are young.
You are young.
You are a teenager.
You are a teenager.
You are old.
You are old.
You are old.


Now i am writing programs regarding the joy of computing using python

example 1:


