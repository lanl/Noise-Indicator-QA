## Fixed problems

This directory contains the fixed problems that are executed on the quantum annealer. 
This includes the graph problems, the Maximum Clique QUBO's for those graph's, and the noise indicator QUBOs. 
These QUBO's can be parsed into python using the following code snippet:

```
import ast

file = open("Advantage_system4.1_N177_MaxClique_QUBO.txt", "r")
QUBO = ast.literal_eval(file.read())
file.close()
print(QUBO)
```


