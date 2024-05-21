
# Operadores Lógicos da Lógica Proposicional

Os operadores lógicos são ferramentas essenciais na lógica proposicional, usados para formar proposições compostas a partir de proposições simples, o que permite a análise de expressões como verdadeiras ou falsas. Abaixo, uma explicação detalhada de cada operador com exemplos e tabelas verdade:

## 1. Conjunção (E, ∧)
A conjunção é um operador lógico que resulta em verdadeiro **somente** se ambas as proposições envolvidas forem verdadeiras.

**Exemplo**: `p ∧ q` é verdadeiro se `p = verdadeiro` e `q = verdadeiro`.

### Tabela Verdade
| p     | q     | p ∧ q |
|-------|-------|-------|
| V     | V     | V     |
| V     | F     | F     |
| F     | V     | F     |
| F     | F     | F     |

## 2. Disjunção (OU, ∨)
A disjunção é verdadeira se **pelo menos** uma das proposições for verdadeira.

**Exemplo**: `p ∨ q` é verdadeiro se `p = verdadeiro`, `q = verdadeiro`, ou ambos.

### Tabela Verdade
| p     | q     | p ∨ q |
|-------|-------|-------|
| V     | V     | V     |
| V     | F     | V     |
| F     | V     | V     |
| F     | F     | F     |

## 3. Negação (NÃO, ¬)
A negação inverte o valor de verdade da proposição.

**Exemplo**: Se `p = verdadeiro`, então `¬p = falso`.

### Tabela Verdade
| p     | ¬p    |
|-------|-------|
| V     | F     |
| F     | V     |

## 4. Condicional (SE...ENTÃO, →)
O operador condicional ou implicação é verdadeiro, exceto quando a primeira proposição é verdadeira e a segunda é falsa.

**Exemplo**: `p → q` implica que se `p = verdadeiro` então `q` deve ser também verdadeiro para que a expressão seja verdadeira.

### Tabela Verdade
| p     | q     | p → q |
|-------|-------|-------|
| V     | V     | V     |
| V     | F     | F     |
| F     | V     | V     |
| F     | F     | V     |

## 5. Bicondicional (SE E SOMENTE SE, ↔)
O bicondicional é verdadeiro quando ambas as proposições têm o mesmo valor de verdade.

**Exemplo**: `p ↔ q` é verdadeiro se ambos `p` e `q` são verdadeiros ou ambos são falsos.

### Tabela Verdade
| p     | q     | p ↔ q |
|-------|-------|-------|
| V     | V     | V     |
| V     | F     | F     |
| F     | V     | F     |
| F     | F     | V     |

Estes operadores são fundamentais para a construção de argumentos e para a realização de deduções lógicas em diversas áreas como matemática e ciência da computação.
