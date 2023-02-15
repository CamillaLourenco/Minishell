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

-
-
-
shell deve:

• Exibir um prompt ao esperar por um novo comando.

• Ter um histórico de trabalho.

• Procurar e lançar o executável correto (com base na variável PATH ou usando um caminho relativo ou absoluto).

• Não utilizar mais de uma variável global. Pense nisso. Você terá que explicar o propósito dela.

• Não interpretar aspas não fechadas ou caracteres especiais que não são exigidos pelo assunto, como \ (barra invertida) ou ; (ponto e vírgula).

• Manipular ' (aspas simples) que deve impedir a shell de interpretar os metacaracteres na sequência entre aspas.

• Manipular " (aspas duplas) que deve impedir a shell de interpretar os metacaracteres na sequência entre aspas, exceto pelo $ (sinal de dólar).

• Implementar redirecionamentos:

◦ < deve redirecionar a entrada.

◦ > deve redirecionar a saída.

◦ << deve ser fornecido um delimitador e, em seguida, ler a entrada até que uma linha contendo o delimitador seja vista. No entanto, isso não precisa atualizar o histórico!

◦ >> deve redirecionar a saída no modo de anexação.

• Implementar tubos (caractere |). A saída de cada comando no pipeline é conectada à entrada do próximo comando por meio de um tubo.

• Manipular variáveis de ambiente ($ seguido de uma sequência de caracteres) que devem se expandir para seus valores.

• Manipular $? que deve se expandir para o status de saída do pipeline em primeiro plano executado mais recentemente.

• Manipular ctrl-C, ctrl-D e ctrl-\ que devem se comportar como no bash.
• No modo interativo:
◦ ctrl-C exibe um novo prompt em uma nova linha.
◦ ctrl-D sai da shell.
◦ ctrl-\ não faz nada.
• Sua shell deve implementar os seguintes comandos internos:
◦ echo com a opção -n
◦ cd com apenas um caminho relativo ou absoluto
◦ pwd sem opções
◦ export sem opções
◦ unset sem opções
◦ env sem opções ou argumentos
◦ exit sem opções
A função readline() pode causar vazamentos de memória. Você não precisa corrigi-los. Mas isso não significa que seu próprio código, sim, o código que você escreveu, possa ter vazamentos de memória.
