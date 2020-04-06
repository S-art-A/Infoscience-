# refelction Apr/6
still dont know how to add other conditions yet 

# definition of variables 
x = [300, 200]# a list, which is a collection of values
y = [300, 200]

def setup():
    size(500,500)
    
def draw():
    global x, y
    background(255)
    strokeWeight(2)
    
    #create 1st indivisual
    for i in range(2):
        circle(x[i], y[i], 40)
        x[i] = x[i] + random(-10,10)
        y[i] = y[i] + random(-10,10)
    
    #bounderies conditions 
    if x[i] > 500:
        x[i] = 500
 
    delay(100)
