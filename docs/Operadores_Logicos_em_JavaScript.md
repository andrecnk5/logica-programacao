
# Operadores Lógicos em JavaScript e Tabelas Verdade

## Conjunção (AND)
O operador `&&` retorna `true` se ambas as condições forem verdadeiras.

**Exemplo**: Mônica usa o Sansão para bater no Cebolinha se ele tentar roubar o Sansão e chamar ela de "gorducha".
```javascript
let tentouRoubarSansao = true;
let chamouDeGorducha = true;
let usaSansao = tentouRoubarSansao && chamouDeGorducha;
console.log("Mônica usa o Sansão:", usaSansao);
```

### Tabela Verdade
| tentouRoubarSansao | chamouDeGorducha | Resultado |
|--------------------|------------------|-----------|
| true               | true             | true      |
| true               | false            | false     |
| false              | true             | false     |
| false              | false            | false     |

## Disjunção (OR)
O operador `||` retorna `true` se pelo menos uma das condições for verdadeira.

**Exemplo**: Cascão participa de um plano se ele acreditar que não envolve água ou se o Cebolinha o convencer de que é seguro.
```javascript
let planoSemAgua = false;
let cebolinhaConvenceu = true;
let participaDoPlano = planoSemAgua || cebolinhaConvenceu;
console.log("Cascão participa do plano:", participaDoPlano);
```

### Tabela Verdade
| planoSemAgua | cebolinhaConvenceu | Resultado |
|--------------|--------------------|-----------|
| true         | true               | true      |
| true         | false              | true      |
| false        | true               | true      |
| false        | false              | false     |

## Negação (NOT)
O operador `!` inverte o valor de verdade da condição.

**Exemplo**: Cascão só entra em pânico se não for garantido que não haverá água.
```javascript
let garantidoSemAgua = false;
let entraEmPanico = !garantidoSemAgua;
console.log("Cascão entra em pânico:", entraEmPanico);
```

### Tabela Verdade
| garantidoSemAgua | Resultado |
|------------------|-----------|
| true             | false     |
| false            | true      |

## Implicação
Em JavaScript, a implicação pode ser representada usando `!p || q`.

**Exemplo**: Se Magali vê uma melancia, então ela vai comer a melancia.
```javascript
let veMelancia = true;
let comeMelancia = veMelancia;  // Simplificado para demonstração
console.log("Magali come a melancia:", comeMelancia);
```

### Tabela Verdade
| veMelancia | comeMelancia | Resultado |
|------------|--------------|-----------|
| true       | true         | true      |
| true       | false        | false     |
| false      | true         | true      |
| false      | false        | true      |

## Bicondicional
O bicondicional pode ser representado como `(p && q) || (!p && !q)`.

**Exemplo**: Mônica e Magali vão ao cinema juntas se e somente se for um filme de aventura.
```javascript
let monicaQuerVer = true;
let magaliQuerVer = true;
let vaoJuntas = (monicaQuerVer && magaliQuerVer) || (!monicaQuerVer && !magaliQuerVer);
console.log("Mônica e Magali vão juntas ao cinema:", vaoJuntas);
```

### Tabela Verdade
| monicaQuerVer | magaliQuerVer | Resultado |
|---------------|---------------|-----------|
| true          | true          | true      |
| true          | false         | false     |
| false         | true          | false     |
| false         | false         | true      |

