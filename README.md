# Chapter5-Exercises
# 1
days = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday']
d = int(input("Please enter the day number between 0 to 6 "))
def dayname(n):
    print(days[n])
dayname(d)

#2
days = {1:'Sunday', 2:'Monday', 3:'Tuesday', 4:'Wednesday', 5:'Thursday', 6:'Friday', 7:'Saturday', }
Start = int(input("Please enter the starting day"))
Length = int(input("Please enter the amount of days spent away"))
R = (Length + Start) %7

def returnday(n):
    print(days[n])

returnday(R)

#3
a <= b
a < b
a < 18 and day != 3
not (3 >= 4)

#4
3 == 3
True
3 != 3
False
3 >= 4
True
not (3 < 4)
False

#5
True
True
True
True
True
True
False
True

#6 I don't know what I did wrong 

GradeBoundary = {75-100:"First", 70-75:"Upper Second", 60-70:"Second", 50-60:"Third", 45-50:"F1 Supp", 40-45:"F2", 0-40:"F3"}

E = int(input("Please enter the mark out of 100"))

def Grades(n):
    print(GradeBoundary[n])
Grades(E)

#7 and #8 and #9
import turtle
def draw_bar(t, height):
    t.begin_fill()
    t.left(90)
    t.forward(height)
    if height < 0:
        t.penup()
        t.forward(-15)
        t.write("  "+ str(height))
        t.forward(15)
        t.pendown()
    else:
        t.write("  "+ str(height))
    t.right(90)
    t.forward(40)
    t.right(90)
    t.forward(height)
    t.left(90)
    t.end_fill()
    t.penup()
    t.forward(10)
    t.pendown()

wn = turtle.Screen()
wn.bgcolor("lightgreen")

tess = turtle.Turtle()
tess.color("blue", "red")
tess.pensize(3)

xs = [-50,48,117,200,240,160,260,220]

for a in xs:
    if a>200:
        tess.color("blue", "red")
    elif a >= 100:
            tess.color("blue", "yellow")
    else:
        tess.color("blue", "green")
    draw_bar(tess, a)

wn.mainloop()

#10
import math

L1 = float(input("Please enter the length of one side of the triangle: "))
L2 = float(input("Please enter the length of the other side of the triangle: "))

def findhypo(a,b):
    Hypo = L1**2 + L2**2
    Hypo2 = math.sqrt(Hypo)
    return (Hypo2)
print(findhypo(L1,L2))

#11
import math

L1 = float(input("Please enter the length of one side of the triangle: "))
L2 = float(input("Please enter the length of the other side of the triangle: "))
L3 = float(input("Please enter the length of the other side of the triangle: "))

def isrightangle(a,b,c):
    Hypo = L1**2 + L2**2
    Hypo = math.sqrt(Hypo)
    if L3 == Hypo:
        print(True)
    else:
        print(False)

print(isrightangle(L1,L2,L3))

#12 I have no idea what to do here
import math

L = float(input("Please enter the length of one side of the triangle: "))
L = float(input("Please enter the length of the other side of the triangle: "))
L = float(input("Please enter the length of the other side of the triangle: "))

def isrightangle(a,b,c):
    Hypo = L**2 + L**2
    Hypo = math.sqrt(Hypo)
    if L == Hypo:
        print(True)
    else:
        print(False)

print(isrightangle(L,L,L))

#13
import math
a = math.sqrt(2.0)
print(a, a*a)
print(a*a == 2.0)
