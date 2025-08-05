# Módulo 01 - Desafio: Criando as Cartas do Super Trunfo

## 1. Sobre o Desafio

Este projeto foi desenvolvido como parte do primeiro módulo da disciplina. O objetivo era construir a base de um jogo de Super Trunfo, criando um sistema em C para cadastrar as informações de duas cartas (cidades) via entrada do usuário e, em seguida, exibir esses dados de forma organizada na tela.

O desafio foca nos conceitos fundamentais da linguagem C:
- Declaração e uso de variáveis de diferentes tipos (`char`, `int`, `float`, `arrays de char`).
- Utilização das funções de entrada e saída padrão (`printf`, `scanf`, `fgets`, `getchar`).
- Formatação de saída de dados.

---

## 2. Requisitos do Desafio

### Requisitos Funcionais
- O programa deve ler os dados de duas cartas (Estado, Código, Cidade, População, Área, PIB, Pontos Turísticos).
- Os dados lidos devem ser armazenados em variáveis apropriadas.
- O programa deve exibir os dados de cada carta de forma clara e organizada.

### Requisitos Não Funcionais
- **Usabilidade:** O programa deve ter instruções claras para o usuário.
- **Legibilidade:** O código deve ser bem indentado e com nomes de variáveis significativos.
- **Simplicidade:** O código não deve utilizar estruturas de repetição (`for`, `while`) ou de decisão (`if`, `else`), sendo uma sequência linear de instruções.

---

## 3. Solução Implementada

O programa `supertrunfo.c` foi escrito em C puro e segue estritamente os requisitos.

- **Fluxo do Programa:** A execução é sequencial. Primeiro, o programa solicita todos os dados da Carta 1, depois todos os dados da Carta 2 e, finalmente, exibe um resumo completo de ambas as cartas cadastradas.
- **Tratamento de Entrada:** Foi dada atenção especial ao tratamento do buffer de entrada do teclado. A função `getchar()` é usada estrategicamente para consumir o caractere de nova linha (`\n`) deixado pelo `scanf`, garantindo que a leitura de strings com `fgets` (necessária para nomes de cidades com espaços) funcione corretamente.

---

## 4. Como Compilar e Executar

Para compilar e executar o projeto, é necessário ter um compilador C, como o GCC (MinGW no Windows).

1.  **Navegue até a pasta do projeto** pelo terminal:
    ```bash
    cd modulo-01-super-trunfo
    ```

2.  **Compile o código-fonte** para gerar um arquivo executável:
    ```bash
    gcc supertrunfo.c -o supertrunfo.exe
    ```

3.  **Execute o programa**:
    ```bash
    ./supertrunfo.exe
    ```