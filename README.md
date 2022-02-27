# Recursividad

# Ejercicio 1

```

def dicotonomia_recursiva(tabla,t):
  i = 0
  j = len(tabla)
  if i > j:
    return "Ausente"
  else:
    n = (init(i+j)/2)
    if tabla[n] == t:
      return n
    else:
      if tabla[n] < int(t):
        print(dicotonomia_recursiva(tabla,t))
        return dicotonomia_recursiva(tabla[i:n-1], t)

def dicotonomia(tabla,t):
  return dicotonomia_recursiva (tabla,t)

if __name__ == "_main__":
  tabla = [4,2,6,3,8,7,5,9,1,0]
  t = input("Introduce un dato")
  print (.format(t, dicotonomia(tabla,t)))
  ```

# Ejercicio 2

```

palabra = str(input("Introduce una palabra"))

class verification:
  def _init_(self,palabra):
    self.palabra = palabra
  def palabra_palindroma(self):
    if str(self.palabra) == str(self.palabra)[::-1]:
      print("Correcto, la palabra es palindroma")
    else:
      print("Falso, la palabra no es palindroma")
resultado = verification(palabra)
print(resultado.palabra_palindroma)

pal = palabra
class convertidor:
  def _init_(self,pal):
    self.pal=pal
  def convertit_mayuscula(self):
    if pal.islower():
      return pal.upper()
    else:
      print (pal)
```

    
# Ejercicio 3


```

bandera = ["R","A","A","R","V","A","A","R","A","R","R","V","R","R","A","V","V"]
rojo = []
verde=[]
azul=[]

class organizacion:
  def __init__(self,bandera,rojo,verde,azul):
    self.bandera=bandera
    self.rojo=rojo
    self.verde=verde
    self.azul=azul
def reorganizar_colores(self):
    if len (self.bandera) > 0:
      color = self.bandera.pop(0)
  if color == "R":
      self.rojo.append(color)
      return self.bandera
    if color == "A":
      self.azul.append(color)
      return self.bandera
    if color == "V":
      self.verde.append(color)
      return self.bandera
    else:
        resultado_bandera=rojo+verde+azul
        print('La bandera ordenada es : {resultado_bandera}')
resultado=organizacion(bandera,rojo,verde,azul)
print(resultado.reorganizar_colores)

```
