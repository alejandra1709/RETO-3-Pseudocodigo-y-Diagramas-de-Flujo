# RETO-3-Pseudocodigo-y-Diagramas-de-Flujo

```pseudocode
n : entero
m : entero
inicio
  m := 2
  Mientras (m <= n**0.5 + 1) hacer
    n/m
    Si modulo (n,m) == 0 entonces
      escribir ("n no es un numero primo")
    sino
      escribir ("m no es divisor de n, n puede ser primo")
      m := m+1
      Si (m >= n**0.5) entonces
        escribir ("n es un numero primo")
  Fin Mientras
fin
```

```mermaid
flowchart TD
    A("INICIO") -->B["n: entero"]
    B --> C["m: entero"]
    C -->D["m=2"]
    D -->E["ejecutar n/m"]
    E -->F{"¿modulo n/m = 0?"}
    F -->|"True"| G["n no es un numero primo"]
    G -->H("FIN")
    F -->|"False"| I["m no es dividor de n"]
    I --> J["m=m+1"]
    J --> K{"¿m es menor o igual a la raiz de n?"}
    K --> |"True"| E
    K --> |"False"| L["n es un numero primo"]
    L -->H
```
