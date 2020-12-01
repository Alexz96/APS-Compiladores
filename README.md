# APS-Compiladores
Repositório para o desenvolvimento do Chat da APS de Compiladores, feito com uso do Antlr

# Integrantes do Grupo
Alexsander Oliveira e Tailine Wornath

# Instruções para execução
1 - Via terminal, localizar a pasta em que o projeto foi extraído e acessar a mesma:
        Exemplo: cd /Downloads/APS-Compiladores

2 - Caso não possuir o ANTLR instalado em seu sistema rodar o comando no terminal Linux/Bash: 
        curl -LO http://www.antlr.org/download/antlr-4.8-complete.jar

3 - Copiar a Lib do ANTLR através do comando abaixo para salvar no diretório de Libs gerais:
        sudo cp antlr-4.7.2-complete.jar /usr/local/lib/

4 - Executar o comando: 
        export CLASSPATH=".:$PWD/antlr-4.8-complete.jar:$CLASSPATH"

Caso desejar, testar o funcionamento do ANTLR executando os comandos abaixo:
    java -jar antlr-4.8-complete.jar
    java org.antlr.v4.Tool

Também, caso desejar, criar um alias para execução do ANTLR
    alias antlr4='java -jar antlr-4.8-complete.jar'

5 - Executar o comando: 
        antlr4 Chat.g4
        Se não possuir o alias, executar java -jar antlr-4.8-complete.jar Chat.g4

6 - Rodar o comando do Java:
        javac *.java

7 - Adicionar o alias para a ferramenta de teste do ANTLR:
        alias grun='java org.antlr.v4.runtime.misc.TestRig'

8 - Executar o comando:
        grun Chat r -tokens

9 - Realizar a conversa conforme desejar e então ao final, pressionar Ctrl+D ou Command+D

# Considerações

O código desenvolvido, deverá reconhecer tokens configurados e então listá-los com seu respectivo tipo.

Referente ao projeto JAVA, que consta no diretório como JavaChat, teve-se por início o desenvolvimento utilizando-se o MAVEN e o Netbeans, mas o mesmo não pôde ser completamente testado para verificar a funcionalidade. Ao se seguir o Tutorial houveram dúvidas, das quais não puderam ser completamente sanadas.

Em partes de testes, houveram erros de código, dos quais ao se buscar nas referências das aulas de compiladores e nas breves gramáticas desenvolvidas, puderam ser resolvidos.