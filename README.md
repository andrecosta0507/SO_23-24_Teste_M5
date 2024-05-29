# Teste de Sistemas Operativos - Módulo 5

Faz *fork* do repositório para teres a tua cópia.

Preenche o ficheiro README diretamente no GitHub. A partir da página principal do repositório, clica em "Edit File" (ícone representando um lápis).

Escreve as respostas dentro dos blocos correspondentes. Substitui as reticências pelo que é pedido em cada pergunta. Não desformates o documento.

Quando acabares, carrega no botão "Commit Changes".

## Informação do aluno

    Nome: André Costa

## P1 - Para as seguintes questões, assinala a opção correta: (2.5v)

  1. Que comando é usado para definir permissões de execução num script Bash?

    A) chmod +x script.sh
    B) chmod -x script.sh
    C) chmod +r script.sh
    D) chmod -r script.sh
    
    Resposta: A

  2. Como se define um comentário num script Bash?

    A) // comentário
    B) /* comentário */
    C) # comentário
    D) -- comentário
    
    Resposta: C
   
  3. Que comando é usado para adicionar uma linha de texto ao final de um arquivo em Bash?

    A) echo "texto" > arquivo
    B) echo "texto" < arquivo
    C) echo "texto" | arquivo
    D) echo "texto" >> arquivo
    
    Resposta: D

  4. Qual é o comando usado para ler a entrada do utilizador num script Bash?

    A) read
    B) input
    C) get
    D) scan
    
    Resposta: A

  5. Que símbolo é usado para denotar uma variável em Bash?

    A) %
    B) $
    C) &
    D) #
    
    Resposta: B

## P2 - Escreve scripts em Bash para realizar as seguintes instruções: (7.5v)

  1. Exibir a mensagem "Olá, Mundo!" no terminal.

    Resposta:
    echo "Olá, Mundo!"
    
  2. Receber dois números como entrada, e exibir a soma dos dois.

    Resposta: echo "Introduza um numero : " 
               read numero1
              echo " introduza outro numero : "
               read numero2
            Soma=$((numero1 + numero2))
            echo "A soma dos dois numeros é de $numero1 e $numero2 é:$Soma"

  3. Ler um valor numérico e imprimir uma mensagem a informar se o mesmo é par ou ímpar.

    Resposta: echo "introduza um numero: "
                read numero1
               if(( numero1 % 2 == 0));
                   echo" O numero é par "
                 else
( echo" o numero é impar")
                
## P3 - Indica o que é realizado pelas seguintes instruções: (6v)

  1. 
    
    echo "scale=2;22/7" | bc

    Resposta:
    imprime  a expressao expressao 22/7  com duas casas decimais
     
  2. 
    
    #!/bin/bash
    sum=0
    for i in {1..5}
    do
      sum=$((sum + i))
    done
    echo "A soma dos números de 1 a 5 é $sum."


    Resposta:
    gera dois numeros e faz a soma dos mesmos.

  3. 
    
    #!/bin/bash
    num=10
    while [ $num -gt 0 ]
    do
      echo "Número: $num"
      ((num--))
    done

    Resposta: o script imprime numeros de 1 a 10  decrementando 1 a 10
    

## P4 - Realiza os seguintes exercícios, com respostas detalhadas: (4v)

  1. O que é um **shebang** (#!) e qual é a sua função num script?

    Resposta:
   O shebang é a sequência "#!" no início de um script seguido do caminho para o interpretador. Ele informa ao sistema operacional qual interpretador deve ser usado para executar o script. Isso permite que você execute scripts de diferentes linguagens sem precisar especificar o interpretador toda vez que o script é executado.

  2. Como se utiliza a instrução 'if-else' num script Bash? Escreve um exemplo simples.

    Resposta:f [ condição ]
then
        # Faz alguma coisa
elif [ condição ]; then
        # Faz outra coisa
else
        do # Faz algo por predefinição
fi
x\    
    
