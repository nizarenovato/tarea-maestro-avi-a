# tarea-maestro-avi-a
trabajo pedido en clases
#Realiza funciones que manejen listas para procesar datos y obtener información.
#Elabora un programa que lea una lista de 10 calificaciones, el programa deberá imprimir los promedios superiores a 8.5.
#Realize el programa haciendo una función que le a los 10 elemntos
#Realize una función que imprima los promedios superiores a 8.5

def pedircalificaciones():
    calificaciones = []
    print("Escribe 10 calificaciones (del 0 al 10):")
    for i in range(10):
        nota = float(input(f"Calificación {i+1}: "))
        calificaciones.append(nota)
    return calificaciones


def mostrar_altas(lista):
    print("\nCalificaciones mayores a 8.5:")
    for nota in lista:
        if nota > 8.5:
            print(nota)
calificaciones = pedircalificaciones()
mostrar_altas(calificaciones)
