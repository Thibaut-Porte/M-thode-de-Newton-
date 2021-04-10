### Methode de Newton ###
import math as m

### 1 ###
print ("1 :")
def f1(x):
    return x**4+3*x-9

def fder(x):
    return (4*x**3)+3

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew, n

print("f1+ = ",Newton(f1, fder, 1.5, 10**(-10), 100000))
print("f1- = ",Newton(f1, fder, -1.5, 10**(-10), 100000))


### 2 ###
print ("2 :")

def f2(x):
    return x-3*m.cos(x)+2

def fder(x):
    return 1+3*m.sin(x)

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f2+ = ",Newton(f2, fder, 1, 10**(-10), 100000))
print("f2.1- = ",Newton(f2, fder, -0.5, 10**(-10), 100000))
print("f2.2- = ",Newton(f2, fder, -4, 10**(-10), 100000))

### 3 ###
print ("3 :")
def f3(x):
    return x*m.exp(x)-7 

def fder(x):
    return (m.exp(x))*(x+1)

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f3 = ",Newton(f3, fder, 1.5, 10**(-10), 100000))


### 4 ###
print ("4 :")
def f4(x):
    return m.exp(x) -x -10

def fder(x):
    return m.exp(x) -1

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f4+ = ",Newton(f4, fder, 3 , 10**(-10), 100000))
print("f4- = ",Newton(f4, fder, -10 , 10**(-10), 100000))



### 5 ###
print ("5 :")
def f5(x):
    return 2*m.tan(x)-x-5

def fder(x):
    return 2/m.cos(x)**2-1

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f5 = ",Newton(f5, fder, 2.1, 10**(-10), 100000))

### 6 ###
print ("6 :")

def f6(x):
    return m.exp(x)- x**2 - 3

def fder(x):
    return m.exp(x)- 2*x

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f6 = ",Newton(f6, fder, 1.9, 10**(-10), 100000))


### 7 ###
print ("7 :")
def f7(x):
    return 3*x+4*m.log(x)-7

def fder(x):
    return 3 + (4/x)

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew ,n

print("f7 = ",Newton(f7, fder, 1.9, 10**(-10), 100000))

### 8 ###
print ("8 :")
def f8(x):
    return x**4 - 2*x**2 +4*x-17

def fder(x):
    return 4*x**3 - 4*x +4

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f8+ = ",Newton(f8, fder, 2.5, 10**(-10), 100000))
print("f8- = ",Newton(f8, fder, -2.5, 10**(-10), 100000))



### 9 ###
print ("9 :")
def f9(x):
    return m.exp(x)- 2*m.sin(x)- 7

def fder(x):
    return m.exp(x)- 2*m.cos(x)

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f9 = ",Newton(f9, fder, 2, 10**(-10), 100000))


### 10 ###
print ("10 :")
def f10(x):
    return (m.log(x**2 + 4))*(m.exp(x))- 10

def fder(x):
    return ((2*x)/(x**4+4))*(m.exp(x))+ (m.log(x**2+4))*(m.exp(x))

def Newton(f, fder,x0, epsilon, Nitermax ):
    xold = x0
    n = 1
    xnew = xold - f(xold)/f(xold)
    diff = xnew - xold
    xold = xnew
    
    while abs(diff) > epsilon and n < Nitermax:
        xnew = xold - (f(xold)/fder(xold))
        diff = xnew - xold
        xold = xnew
        n += 1
    return xnew , n

print("f10 = ",Newton(f10, fder, 1.5, 10**(-10), 100000))

