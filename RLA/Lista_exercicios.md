 # UNIFOR
**Disciplina:** Raciocínio lógico algorítmico 
**Orientador:** Professor Ricardo Carubbi

## Lista de exercícios

### Exercício 03
Represente, em fluxograma e pseudocódigo, um algoritmo para determinar se um número inteiro e positivo é par ou ímpar.
#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite um número}}
B --> C[/Número/]
C --> D{Número > 0}
D --NÃO--> E{{O número informado é negativo!}}
D --SIM--> F[resto = número % 2]
F --> G{resto == 0}
E --> Z([FIM])
G --NÃO--> H{{O número é impar!}}
G --SIM--> I{{O número é par!}}
H --> Z
I --> Z
```
#### Pseudocódigo
```
1 ALGORITMO verifica_par_impar
2 DECLARE número resto NUMERICO
3 ESCREVA "Digite um número"
4 LEIA numero
5 SE numero > 0 ENTAO
6   resto = numero % 2 
7   SE resto == 0 ENTAO
8     ESCREVA "O numero é par!"
9   SENAO
10      ESCREVA "O número é impar!"
11 SENAO
12     ESCREVA "O número deve ser positivo!"
FIM_ALGORITMO
```
