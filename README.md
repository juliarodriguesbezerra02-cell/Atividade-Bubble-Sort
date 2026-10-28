# Atividade-Bubble-Sort
# Classificação de Tempos de Entrega com Bubble Sort (C)

**Instituição:** UDF – Centro Universitário do Distrito Federal
**Disciplina:** Algoritmos e Pensamento Computacional
**Professora:** Profa. Karla R. Sartin

## Integrantes e contribuições

| Integrante | Contribuição no projeto |
|---|---|
| Júlia Rodrigues Bezerra  | Estrutura inicial do programa, array de dados e `.gitignore` |
| Nicole Moreira de Albuquerque  | Cabeçalho, critério de ordenação e exibição dos dados antes da ordenação |
| Matheus Mendes dos Santos  | Implementação do algoritmo Bubble Sort com comentários |
| Rafael Oliveira da Silva  | Exibição dos dados após a ordenação e dos tempos mínimo e máximo |
| Roberto Rosado  | Documentação (`README.md`) e exemplo de entrada e saída |

## Problema escolhido

Uma empresa de delivery registra o tempo (em minutos) de cada entrega realizada. Com os tempos desorganizados, fica difícil identificar quais entregas foram mais rápidas e quais demoraram mais. A ordenação dos dados permite analisar o desempenho do serviço, encontrar atrasos e apoiar decisões, como rever rotas ou o número de entregadores.

## Objetivo da aplicação

Organizar, em ordem **crescente** (do menor para o maior), os tempos de entrega de 10 pedidos usando o algoritmo Bubble Sort, mostrando os dados antes e depois da ordenação.

## Como o Bubble Sort funciona

O Bubble Sort (ordenação por bolha) compara elementos vizinhos do vetor e troca os de posição quando o da esquerda é maior que o da direita. A cada passada completa pelo vetor, o maior valor "sobe como uma bolha" até o final. O processo se repete até que todo o vetor esteja ordenado.

No código, o laço externo controla as passadas, o laço interno compara os vizinhos e a troca é feita com uma variável auxiliar (`temp`):

```c
if (tempos[j] > tempos[j + 1]) {
    temp = tempos[j];
    tempos[j] = tempos[j + 1];
    tempos[j + 1] = temp;
}
```

## Como compilar e executar

Requisito: compilador C (por exemplo, GCC).

```bash
gcc bubble_sort_entregas.c -o bubble_sort_entregas
./bubble_sort_entregas
```

No Windows, execute `bubble_sort_entregas.exe`. Também é possível abrir o arquivo no OnlineGDB, no Code::Blocks ou no Visual Studio Code.

## Exemplo de entrada e saída

**Entrada:** os dados estão definidos no próprio código, no vetor `tempos` (em minutos):

```
35 20 48 15 42 28 55 18 31 25
```

**Saída no terminal:**

```
=== Classificacao de tempos de entrega ===
Criterio: ordem CRESCENTE (do menor para o maior)

Tempos ANTES da ordenacao (minutos):
35 20 48 15 42 28 55 18 31 25 

Tempos DEPOIS da ordenacao (minutos):
15 18 20 25 28 31 35 42 48 55 

Entrega mais rapida: 15 minutos
Entrega mais demorada: 55 minutos
```

## Tecnologias e ferramentas

- Linguagem C
- Compilador GCC
- Git e GitHub (versionamento)
- [EDITOR/IDE USADO PELO GRUPO]

## Considerações finais


