'''Declarion de Variables'''

ruta=0

precio_tiquete=0

asiento=0

add=1
asientos_disponibles=0
rutas = ["San Jose - Puntarenas","San Jose - Guancaste","San Jose - Limón","San Jose - Alajuela","San Jose - Heredia"]
rutas2 = [["San Jose - Puntarenas",4500],["San Jose - Guancaste",5500],["San Jose - Limón",6000],["San Jose - Alajuela",800],["San Jose - Heredia",550]]

print(rutas[4])

print("********COMPRE SU TIQUETE******")
   
while add == 1:
    for x in range (len(rutas)):
        print(x+1,"-", rutas[x])

    ruta = int(input("Seleccione la ruta\n"))

    print(f"\n1. Ida (₡{rutas2[ruta-1][1]}) ")
    print(f"2. Ida y vuelta (₡{rutas2[ruta-1][1]*2})")
    precio_tiquete = int(input("Seleccione el tiquete\n"))
    print("\n")
    for i in range (11):
       print (i, end = ' ')
    asiento = int(input("\nSeleccione el asiento\n"))
    
   
    add = int(input("\nDesea salir: Si(2)  No (1) \n"))

    
    print("------------------------COMPRA EXITOSA---------------")
    print("Asiento  ",asiento)
    print("La ruta seleccionada fue  ",rutas2[ruta-1][0])
    print("El precio total fue de ¢",rutas2[ruta-1][1]*precio_tiquete)

