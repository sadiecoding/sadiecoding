def Rect(left, top, width, height, fill='black', border=None, borderWidth=2,
         opacity=100, rotateAngle=0, dashes=False, align='left-top',
         visible=True):
    # Your implementation for Rect goes here

def Oval(centerX, centerY, width, height, fill='black', border=None,
         borderWidth=2, opacity=100, rotateAngle=0, dashes=False,
         align='center', visible=True):
    # Your implementation for Oval goes here

def Circle(centerX, centerY, radius, fill='black', border=None,
           borderWidth=2, opacity=100, rotateAngle=0, dashes=False,
           align='center', visible=True):
    # Your implementation for Circle goes here

def Line(x1, y1, x2, y2, fill='black', lineWidth=2, dashes=False, opacity=100,
         visible=True, arrowStart=False, arrowEnd=False):
    # Your implementation for Line goes here

def RegularPolygon(centerX, centerY, radius, points, fill='black', border=None,
                   borderWidth=2, opacity=100, rotateAngle=0, dashes=False,
                   align='center', visible=True):
    # Your implementation for RegularPolygon goes here

def Star(centerX, centerY, radius, points, fill='black', border=None,
         borderWidth=2, roundness=None, opacity=100, rotateAngle=0,
         dashes=False, align='center', visible=True):
    # Your implementation for Star goes here

def Polygon(*points, fill='black', border=None, borderWidth=2,
            opacity=100, rotateAngle=0, dashes=False, visible=True):
    # Your implementation for Polygon goes here

# Draw Mario
def draw_mario():
    # Head
    Oval(200, 75, 50, 50, fill=skin)

    # Hat
    Rect(175, 50, 100, 25, fill=red)
    Rect(190, 25, 70, 25, fill=red)
    Rect(200, 0, 50, 25, fill=red)

    # Eyes
    Circle(185, 85, 5, fill=white)
    Circle(215, 85, 5, fill=white)
    Circle(185, 85, 3, fill=black)
    Circle(215, 85, 3, fill=black)

    # Nose
    Polygon(200, 90, 205, 100, 195, 100, fill=skin)

    # Mouth
    Line(190, 110, 210, 110, lineWidth=2)

    # Body
    Rect(175, 125, 50, 75, fill=blue)
    Rect(225, 125, 50, 75, fill=blue)

    # Arms
    Rect(150, 125, 25, 50, fill=blue)
    Rect(275, 125, 25, 50, fill=blue)

    # Legs
    Rect(190, 200, 20, 50, fill=blue)
    Rect(230, 200, 20, 50, fill=blue)

# Draw Mario on the canvas
draw_mario()
