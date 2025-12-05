##🧮 Calculadora Simples — Python + Shell Script

Este repositório contém uma calculadora simples desenvolvida em Python,
acompanhada de um script .sh para facilitar a execução em sistemas
Linux.

O objetivo do projeto é demonstrar: - criação de scripts executáveis no
Linux, - permissões de execução (chmod), - interação com o usuário pelo
terminal, - estrutura básica de um programa Python.

------------------------------------------------------------------------

###📁 Estrutura do Repositório

    calculadora/
    ├── calculadora.py        # Código principal em Python
    ├── calculadora.sh        # Script executável para rodar a calculadora
    └── README.md             # Documentação do projeto

------------------------------------------------------------------------

###🚀 Como Executar o Script .sh (Linux)

Siga os passos abaixo para rodar a calculadora através do arquivo
executável.

1. Tornar o arquivo executável

    `chmod +x calculadora.sh`

2. Executar o script

    `./calculadora.sh`

O script irá executar automaticamente o arquivo Python calculadora.py.

------------------------------------------------------------------------

###🐍 Como Executar Diretamente em Python

Se preferir rodar o programa sem o script .sh, use:

    python3 calculadora.py

------------------------------------------------------------------------

###📌 Explicação do Código Python

1. Função converter_para_numero(s)

-   Tenta converter a entrada primeiro para int.
-   Se falhar, tenta converter para float.
-   Se não for possível, informa ao usuário que não é um número válido.

2. Função escolher_operacao()

-   Exibe o menu de operações disponíveis.
-   Recebe a escolha do usuário:
    -   1 → adição
    -   2 → subtração
    -   3 → multiplicação
    -   4 → divisão
    -   Q → sair

3. Função calcular(op, a, b)

-   Executa a operação desejada.
-   Trata o erro de divisão por zero com segurança.

4. Função main()

-   Exibe o menu repetidamente.
-   Solicita os números ao usuário.
-   Converte as entradas usando converter_para_numero().
-   Executa a operação escolhida.
-   Trata erros com try/except.
-   Só termina quando o usuário digita Q.

------------------------------------------------------------------------

###🛠️ Funcionamento do Arquivo .sh

O script contém:

    #!/bin/bash
    python3 calculadora.py

Ele simplesmente: - chama o Bash, - executa o arquivo calculadora.py.

Assim, a calculadora pode ser iniciada com:

    ./calculadora.sh

------------------------------------------------------------------------

###📜 Licença

Projeto desenvolvido para fins educacionais.
Sinta-se livre para copiar, modificar e reutilizar.
