
# Operadores Lógicos em Python e Tabelas Verdade

## Conjunção (AND)
O operador `and` retorna `True` se ambas as condições forem verdadeiras.

**Exemplo**: Mônica usa o Sansão para bater no Cebolinha se ele tentar roubar o Sansão e chamar ela de "gorducha".
```python
tentou_roubar_sansao = True
chamou_de_gorducha = True
usa_sansao = tentou_roubar_sansao and chamou_de_gorducha
print("Mônica usa o Sansão:", usa_sansao)
```

### Tabela Verdade
| tentou_roubar_sansao | chamou_de_gorducha | Resultado |
|----------------------|--------------------|-----------|
| True                 | True               | True      |
| True                 | False              | False     |
| False                | True               | False     |
| False                | False              | False     |

## Disjunção (OR)
O operador `or` retorna `True` se pelo menos uma das condições for verdadeira.

**Exemplo**: Cascão participa de um plano se ele acreditar que não envolve água ou se o Cebolinha o convencer de que é seguro.
```python
plano_sem_agua = False
cebolinha_convenceu = True
participa_do_plano = plano_sem_agua or cebolinha_convenceu
print("Cascão participa do plano:", participa_do_plano)
```

### Tabela Verdade
| plano_sem_agua | cebolinha_convenceu | Resultado |
|----------------|---------------------|-----------|
| True           | True                | True      |
| True           | False               | True      |
| False          | True                | True      |
| False          | False               | False     |

## Negação (NOT)
O operador `not` inverte o valor de verdade da condição.

**Exemplo**: Cascão só entra em pânico se não for garantido que não haverá água.
```python
garantido_sem_agua = False
entra_em_panico = not garantido_sem_agua
print("Cascão entra em pânico:", entra_em_panico)
```

### Tabela Verdade
| garantido_sem_agua | Resultado |
|--------------------|-----------|
| True               | False     |
| False              | True      |

## Implicação
A implicação pode ser representada como `not p or q`.

**Exemplo**: Se Magali vê uma melancia, então ela vai comer a melancia.
```python
ve_melancia = True
come_melancia = ve_melancia  # Simplificado para demonstração
print("Magali come a melancia:", come_melancia)
```

### Tabela Verdade
| ve_melancia | come_melancia | Resultado |
|-------------|---------------|-----------|
| True        | True          | True      |
| True        | False         | False     |
| False       | True          | True      |
| False       | False         | True      |

## Bicondicional
O bicondicional pode ser representado como `(p and q) or (not p and not q)`.

**Exemplo**: Mônica e Magali vão ao cinema juntas se e somente se for um filme de aventura.
```python
monica_quer_ver = True
magali_quer_ver = True
vao_juntas = (monica_quer_ver and magali_quer_ver) or (not monica_quer_ver and not magali_quer_ver)
print("Mônica e Magali vão juntas ao cinema:", vao_juntas)
```

### Tabela Verdade
| monica_quer_ver | magali_quer_ver | Resultado |
|-----------------|-----------------|-----------|
| True            | True            | True      |
| True            | False           | False     |
| False           | True            | False     |
| False           | False           | True      |

