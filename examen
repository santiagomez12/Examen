import math 

g=9.8 
def funcion1(angulo,rozamiento,masa1):
  masa2=0 
  angulo=math.radians(angulo) 
  seno=math.sin(angulo)
  coseno=math.cos(angulo)
  result=[]
  while True:
    aceleracion=g*(masa1*seno-masa2-rozamiento*masa1*coseno)/(masa1+masa2)
    if aceleracion<0:
      result.append([masa2,"cae"])
      break
    else:
      result.append([masa2,"sube"]) 
      masa2+=0.5
  return result
      
print(funcion1(25,0.4,17))

def funcion2(masa1,masa2,rozamiento):
  for angulo in range(10,86):
    angulo=math.radians(angulo)
    seno=math.sin(angulo)
    coseno=math.cos(angulo)
    aceleracion=g*(masa1*seno-masa2-rozamiento*masa1*coseno)/(masa1+masa2)
    
    if aceleracion==0:
      return math.degrees(angulo)
  return -1

print(funcion2(8,3,0.3))
