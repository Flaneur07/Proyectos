# Proyecto: Tienda de Verduras "VerduJuan"

print("Bienvenido a la tienda de Verduras Verdujuan")
print("----Productos----------")
decision = int(input("¿Desea comprar?: [1] Si - [2] No\n"))
frutas = {"manzana":10000, "pera":8000, "banano":5000}
carrito = []
sumatoria = []
compras = 0
contador = 0
import time
while decision == 1: 
  print("")
  print("----Productos----------")
  print("manzana $ 10.000 - pera $ 8.000 - banano $ 5.000:\n")
  
  compra = str(input("¿Qué producto deseas comprar?\n"))
  cantidad = int(input("Cantidad:\n"))
  if compra in frutas:
    carrito.append(frutas[compra] * cantidad)
    sumatoria = sum(carrito)
    print("Costo de Tu Carrito de Compras:\t", compra, carrito)
    contador += 1
    print("Compra:\t", contador)
    time.sleep(2)
    decision = int(input("¿Desea seguir comprando?: [1] Si - [2] No\n"))   
    time.sleep(2)
    if decision == 2:
      print("Has finalizado el proceso de compra")
      print("------CARRITO DE COMPRAS------------")
      print("")
    

