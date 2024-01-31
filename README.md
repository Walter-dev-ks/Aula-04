
# Estudo de Classes em Java - Triângulos

Este projeto é um exemplo de estudo de classes em Java, utilizando o conceito de triângulos.

## Sobre

O código fornecido consiste em duas classes principais: `Main` e `Triangule`. A classe `Main` é responsável pela execução do programa, enquanto a classe `Triangule` representa a entidade do triângulo, incluindo o cálculo de sua área.

## Pré-requisitos

- JDK (Java Development Kit) instalado
- Ambiente de desenvolvimento Java configurado

## Instalação

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/seu-projeto.git
cd seu-projeto
```

2. Compile e execute o código:

```bash
javac Main.java
java Main
```

## Estrutura do Projeto

### `Main.java`

Este arquivo contém a lógica principal do programa. Ele cria instâncias da classe `Triangule`, solicita as medidas dos triângulos X e Y, calcula suas áreas e determina qual triângulo possui a maior área.

### `Triangule.java`

Esta classe define a entidade do triângulo. Ela possui os atributos `a`, `b`, e `c`, que representam os lados do triângulo, e o método `area()`, que calcula a área do triângulo com base nos seus lados.

```java
package entities;

public class Triangule {
    public double a;
    public double b;
    public double c;

    public double area() {
        double p = (a + b + c) / 2.0;
        double result = Math.sqrt(p * (p - a) * (p - b) * (p - c));
        return result;
    }
}
```

## Exemplo

O código solicita as medidas dos triângulos X e Y e exibe a área de cada triângulo, além de indicar qual triângulo possui a maior área.
`Dica`: Use os seguintes valores para testar se seu código está funcionando:

  `Triangulo X:`
  ```bash
    3.00
    4.00
    5.00
```

  `Triangulo Y`
  ```bash
    7.50
    4.50
    4.02
```

  `Resultado`
  
  Triangulo X area: `6.0000`
  
  Triangulo Y area: `7.5638`
