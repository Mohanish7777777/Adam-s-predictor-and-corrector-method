# Adam-s-predictor-and-corrector-method

Evaluate (𝟏. 𝟒) , given that 𝒅𝒚 = 𝒙𝟐(𝟏 + 𝒚), 𝒚(𝟏) = 𝟏, 𝒚(𝟏. 𝟏) = 𝟏. 𝟐𝟑𝟑, 𝒚(𝟏. 𝟐) = 𝟏. 𝟓𝟒𝟖
𝒅𝒙
and 𝒚(𝟏. 𝟑) = 𝟏. 𝟗𝟕𝟗 using Adam’s predictor and corrector method.

Program:
```python3
def f (x, y):
return x**2*(1+y)
x0=float (input ("Enter x0: "))
y0=float (input ("Enter y0: "))
x1=float (input ("Enter x1: "))
y1=float (input ("Enter y1: "))
x2=float (input ("Enter x2: "))
y2=float (input ("Enter y2: "))
x3=float (input ("Enter x3: "))
y3=float (input ("Enter y3: "))
h =0.1
y4p=y3+(h/24) *(55*f(x3,y3)-59*f(x2,y2)+37*f(x1,y1)-9*f(x0,y0))
x4=x3+h
y4c=y3+(h/24) *(9*f(x4,y4p) +19*f(x3,y3)-5*f(x2,y2)+f(x1,y1))
print ("Approximate soln is %0.4f"%y4c)
```
Output:
Enter x0: 1
Enter y0: 1
Enter x1: 1.1
Enter y1: 1.233
Enter x2: 1.2
Enter y2: 1.548
Enter x3: 1.3
Enter y3: 1.979
Approximate solution is 2.5749
