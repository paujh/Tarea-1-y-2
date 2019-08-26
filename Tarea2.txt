import matplotlib.pyplot as plt
#Para este ejercicio consideraremos que las ventas de los boletos del cine fueron al 100%, i.e. los 200 boletos, y que cada boleto cuesta $70. Tambien supondremos que por cliente gasta $45, y que sus costos fijos son de $5000
b = float(input("Escribe tus costos fijos: ")) #5000
#Supondremos que el usuario pone todos los datos en el comentario anterior, incluyendo precios por unidad
m1 = float(input("Escribe tus costos variables: ")) #9000
m2 = float(input("Escribe tus ingresos totales: ")) #14000

if m2 > 0.0:
    if m1 > 0.0:
        if m2 > m1:
            pe = (b/(1-(m1/m2)))/1000
            print("A partir del cliente " + str(pe) + " tendra ganancias.")
            X = [i*1 for i in range(0,10)]
            Y = [m2*i for i in X]
            Z = [(m1*i)+b for i in X]
            plt.figure()
            plt.plot(X, Y, "b-")
            plt.plot(X, Z, "k-")
            plt.xlabel('Numero de cliente')
            plt.ylabel('Dinero $')
            plt.savefig("Ejemplo1.png")
            plt.show

        else: 
          print("No hay ganancias.")
    else:
      print("Datos incorrectos.")
else: 
  print("Datos incorrectos.")
