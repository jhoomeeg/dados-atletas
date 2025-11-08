# Dados dos Atletas

Este é um projeto JavaScript que implementa uma classe `Atleta` para gerenciar informações de atletas, incluindo cálculos de categoria, IMC e média de notas.

## Funcionalidades

A classe `Atleta` possui os seguintes atributos:
- Nome
- Idade
- Peso
- Altura
- Notas

E implementa os seguintes métodos:
- `calculaCategoria()`: Determina a categoria do atleta com base na idade
- `calculaIMC()`: Calcula o Índice de Massa Corporal
- `calculaMediaValida()`: Calcula a média das notas descartando a maior e menor nota
- Métodos getters para todos os atributos e cálculos

## Como utilizar

1. Clone este repositório:
```bash
git clone https://github.com/[seu-usuario]/dados-atletas
```

2. Execute o arquivo JavaScript:
```bash
node dados-atletas.js
```

## Exemplo de uso

```javascript
const atleta = new Atleta("Cesar Abascal", 30, 80, 1.70, [10, 9.34, 8.42, 10, 7.88]);

console.log(`Nome: ${atleta.obtemNomeAtleta()}`);
console.log(`Idade: ${atleta.obtemIdadeAtleta()}`);
console.log(`Peso: ${atleta.obtemPesoAtleta()}`);
console.log(`Altura: ${atleta.obtemAlturaAtleta()}`);
console.log(`Notas: ${atleta.obtemNotasAtleta()}`);
console.log(`Categoria: ${atleta.obtemCategoria()}`);
console.log(`IMC: ${atleta.obtemIMC()}`);
console.log(`Média válida: ${atleta.obtemMediaValida()}`);
```

## Saída esperada

```
Nome: Cesar Abascal
Idade: 30
Peso: 80
Altura: 1.7
Notas: 10,9.34,8.42,10,7.88
Categoria: Adulto
IMC: 27.68166089965398
Média válida: 9.25333333
```

## Regras implementadas

### Categorias
- Infantil: 9 a 11 anos
- Juvenil: 12 e 13 anos
- Intermediário: 14 e 15 anos
- Adulto: 16 a 30 anos
- Sem categoria: demais idades

### IMC
Calculado através da fórmula: peso / (altura × altura)

### Média válida
Calculada removendo a maior e menor nota e fazendo a média das notas restantes.

