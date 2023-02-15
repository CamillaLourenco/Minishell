# Minishell

breve explicação de cada um dos termos:

#Lexer (ou analisador léxico) 
é responsável por ler o código-fonte de um programa e converter cada símbolo em uma unidade chamada token. Um token é uma sequência de caracteres que representa uma unidade significativa no código, como uma palavra-chave, nome de variável, operador ou valor literal. O Lexer é a primeira etapa de um compilador ou interpretador, e sua saída é uma sequência de tokens que é passada para a próxima etapa do processo.

#Parser (ou analisador sintático) 
é responsável por analisar a sequência de tokens produzida pelo Lexer e construir uma árvore de análise sintática que representa a estrutura do programa. O Parser verifica se a sequência de tokens segue as regras sintáticas da linguagem de programação, como a ordem dos operadores e a correspondência entre parênteses, chaves e colchetes. A saída do Parser é uma árvore de análise sintática que é usada na próxima etapa do processo de compilação ou interpretação.

#Expander (ou processador de macros) 
é uma ferramenta que permite que os programadores definam suas próprias abstrações e linguagens específicas de domínio, para simplificar a escrita e a leitura do código. As macros são instruções que são definidas pelo programador e podem ser expandidas pelo Expander em outras instruções ou blocos de código, permitindo que o programador escreva código de maneira mais concisa e clara. O Expander é um componente opcional de alguns compiladores e interpretadores.

#Executor (ou interpretador) 
é responsável por executar o código do programa. Ele pode fazer isso diretamente, interpretando as instruções uma a uma, ou pode gerar código de máquina que pode ser executado pelo processador do computador. O Executor é a última etapa de um compilador ou interpretador, e sua saída é a execução do programa, que pode ser uma saída de texto, gráficos, som ou qualquer outra forma de resultado. O interpretador é geralmente mais lento que um compilador, mas pode ser mais fácil de usar para testar e depurar o código.




-

-

- 
//A existência dos shells está ligada à própria existência da Tecnologia da Informação.
Na época, todos os desenvolvedores concordavam que a comunicação com um computador usando chaves de 1/0 era seriamente irritante.
Foi apenas lógico que eles tivessem a ideia de criar um software para se comunicar com um computador usando linhas de comando interativas em uma linguagem um pouco próxima da linguagem humana.
Graças ao Minishell, você poderá viajar no tempo e voltar aos problemas enfrentados pelas pessoas quando o Windows não existia.//
