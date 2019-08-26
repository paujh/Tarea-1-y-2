a = float(input("Escribe un numero: "))
b = float(input("Escribe un segundo numero: "))

print(str(a) + " + " + str(b) + " = " + str(a+b))
print(str(a) + " - " + str(b) + " = " + str(a-b))
print(str(b) + " - " + str(a) + " = " + str(b-a))
print(str(a) + " x " + str(b) + " = " + str(a*b))
if b == 0.0:
  print("La division de " + str(a) + " entre " + str(b) + " es invalida.")
  print(str(b) + " / " + str(a) + " = " + str(b/a))
else:  
  print(str(a) + " / " + str(b) + " = " + str(a/b))
  print(str(b) + " / " + str(a) + " = " + str(b/a))
print(str(a) + " a la " + str(b) + " = " + str(a**b))
print(str(b) + " a la " + str(a) + " = " + str(b**a))
print("La raiz " + str(a) + " de " + str(b) + " = " + str(b**(1/a)))
print("La raiz " + str(b) + " de " + str(a) + " = " + str(a**(1/b)))
