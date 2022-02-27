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
