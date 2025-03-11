import turtle  

# Configuración de la pantalla
pantalla = turtle.Screen()
pantalla.bgcolor("white")

# Configuración de la tortuga
t = turtle.Turtle()
t.speed(3)
t.color("blue")
t.pensize(3)

# Mover la tortuga a la posición inicial
t.penup()
t.goto(0, -150)
t.pendown()

# Función para dibujar un corazón
def dibujar_corazon():
    t.begin_fill()
    t.fillcolor("blue")

    t.left(140)  
    t.forward(180)  
    t.circle(-90, 200)  
    t.left(120)  
    t.circle(-90, 200)  
    t.forward(180)  

    t.end_fill()

# Dibujar el corazón
dibujar_corazon()

# Escribir un mensaje en el centro del corazón
t.penup()
t.goto(-100, -10)
t.color("white")
t.write("Cecyte Comonfort 1", font=("Arial", 18, "bold"))

# Ocultar la tortuga y finalizar
t.hideturtle()
turtle.done()
