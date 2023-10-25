Quadric code
Gives step for quadratic

import math

print("enter your a,b,c values in the form ax2 + bx + c = 0")

#convert values to floats
aValue=float(input("A value:"))

bValue=float(input("B value:"))

cValue=float(input("C value:"))

divide= 2*aValue
#√ sqaure root

print("eqation")
print("%fx^2+%fx+%f=0 " %(aValue,bValue,cValue))
cc=input()
print("Start")
print("-(%f) ± √(%f)2-4(%f)(%f)/2(%f)\n" % (bValue,bValue,aValue,cValue,aValue))
cc=input()

print("First  step -(b)")

#First part -(b)
bNegative=bValue*-1
print("(%f) ± √(%f)2-4(%f)(%f)/%f\n" % (bNegative,bValue,aValue,cValue,divide))
cc=input()

print("Second step b to the power of 2")

#second part (b)**2 to the power of
bPower=bValue**2
print("(%f) ± √(%f)-4(%f)(%f)/(%f)\n" % (bNegative,bPower,aValue,cValue,divide))
cc=input()


#third part-4(2)(-7)
ac= -4*aValue*cValue

print("third step -4(a)(c)")

print("(%f) ± √(%f)+%f/%f\n" % (bNegative,bPower,ac,divide))
cc=input()



#Second part times ac
bac=bPower+ac
xx=math.sqrt(bac)
print("Fourth step √%f+%f" % (bPower,ac))

print("(%f) ± %f/%f\n" % (bNegative,xx,divide))
cc=input()


plusValue=bNegative + xx
yy=plusValue/divide
print("added answer")
print("(%f) + %f/%f=%f\n" % (bNegative,xx,divide,yy))
cc=input()
NegativeValue=bNegative - xx
zz=NegativeValue/divide
print("negative answer")
print("(%f) - %f/%f=%f\n" % (bNegative,xx,divide,zz))
cc=input()
print(" x = %f  " %(yy))
print("x = %f  " %(zz))

