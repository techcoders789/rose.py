# rose.py
code here
import turtle

# Set up the turtle screen
screen = turtle.Screen()
screen.bgcolor("black")

# Create the turtle object
pen = turtle.Turtle()
pen.speed(0)  # Set the turtle speed to the fastest

# Define the RGB color values
red = 1.0
green = 0.0
blue = 0.0

# Rotate and draw the pattern
for _ in range(720):  # 360 degrees divided by 5 degrees
    # Set the RGB color
    pen.color(red, green, blue)

    # Draw a square
    for _ in range(4):
        pen.forward(200)  # Increase the forward distance to make it bigger
        pen.right(90)

    # Rotate the turtle
    pen.right(5)

    # Update the RGB color values
    red -= 0.01
    green += 0.01
    blue += 0.01

# Exit the turtle program
turtle.done()
