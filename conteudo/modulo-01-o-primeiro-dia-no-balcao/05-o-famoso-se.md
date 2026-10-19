# As Regras do Balcão: Tomando Decisões com o Famoso "Se"
> **Uma Aventura Python** — Por Aya Nicodemos (Ayasoft Studios)  
> *Módulo 1: O Primeiro Dia no Balcão — Lição 5*

---

Chegamos a uma das ferramentas mais fascinantes do comércio mágico: a tomada de decisões, conhecida carinhosamente em toda a computação como **o famoso "Se"**.

Até agora, as ordens que passamos para o nosso Golem seguiam sempre em linha reta, do começo ao fim. Mas a vida de um empório movimentado não é uma linha reta!

A cada minuto, você precisa fazer escolhas com base no que o aventureiro traz até o balcão:
* *Se o guerreiro tiver ouro suficiente, entregue a espada mágica.*
* *Senão, avise para ele voltar à masmorra para juntar mais moedas!*

---

### Como funciona a estrutura "Se"?

A estrutura condicional funciona exatamente como se você estivesse fazendo uma pergunta de Sim ou Não para o Golem:

```text
SE (esta condição for Verdadeira):

    Execute estas ordens aqui dentro!


SENÃO:

    Execute este plano alternativo!
```

Vamos ver um caso real no balcão da nossa loja:

> Um guerreiro entra com pressa querendo comprar uma **Espada de Aço** que custa **50 moedas de ouro**.

Veja como o seu Golem ajudante deve analisar a situação, com espaço generoso entre os comandos para você ler com calma:

```text
preco da espada = 50

ouro do guerreiro = 60



SE (ouro do guerreiro >= preco da espada):

    troco = ouro do guerreiro - preco da espada
    
    DIZER: "Parabéns pela compra! Seu troco é de " + troco + " moedas."
    
    ENTREGAR: Espada de Aço



SENÃO:

    DIZER: "Sinto muito, meu nobre! Você precisa de 50 moedas. Volte ao calabouço para juntar mais ouro!"
```

Veja como é elegante e intuitivo:
* Se o guerreiro tiver `60 moedas`, a pergunta `60 >= 50` é **Verdadeira**. O Golem entra no primeiro bloco: calcula o troco de 10 moedas, entrega a espada e festeja a venda!
* Se o guerreiro tiver apenas `35 moedas`, a pergunta `35 >= 50` é **Falsa**. O Golem não entrega a espada de jeito nenhum! Ele pula direto para o bloco do **SENÃO**, avisando educadamente que faltam moedas.

O seu comércio agora tem inteligência própria: ele avalia a carteira do cliente e protege o seu estoque!

---

### E quando temos opções variadas? (O "Senão Se")

Nem tudo na loja é preto no branco. Às vezes, você quer aplicar a política de descontos da guilda dependendo de quem está no balcão:
* Se for um **Mago**, dê 20% de desconto em poções de mana.
* Senão, se for um **Clérigo**, dê 15% de desconto em elixires de cura.
* Senão, se for um **Bárbaro**, dê uma tocha grátis de brinde.
* Senão (qualquer outra classe), cobre o preço normal de tabela.

Na programação, essa sequência de opções intermediárias se chama **"Senão Se"**:

```text
SE (classe do heroi == "Mago"):

    desconto = 0.20
    DIZER: "Desconto arcano de 20% aplicado!"



SENÃO SE (classe do heroi == "Clérigo"):

    desconto = 0.15
    DIZER: "Bênção da catedral com 15% de desconto!"



SENÃO SE (classe do heroi == "Bárbaro"):

    desconto = 0.0
    DIZER: "Tome uma tocha de brinde para iluminar sua caverna!"



SENÃO:

    desconto = 0.0
    DIZER: "Preço padrão de tabela aplicado."
```

O Golem lê essa lista de cima para baixo. No primeiro teste que for Verdadeiro, ele aplica a ordem e ignora todo o restante da fila de condições!

---

### O Segredo da Indentação (O Recuo das Gavetas)

Repare com atenção que as instruções que devem acontecer dentro do `SE` estão um pouquinho "empurradas" para a direita com alguns espaços de margem.

Esse recuo visual se chama **Indentação**.

Pense na indentação como uma gaveta que foi aberta: tudo o que estiver dentro daquele recuo para a direita só vai acontecer se aquela gaveta específica for aberta!

O Python é famoso no mundo inteiro exatamente por isso: ele não usa chaves ou pontuações confusas para delimitar blocos; ele usa a beleza da organização visual!

Agora o seu Golem já sabe pensar e escolher. Mas o que fazer quando há uma fila imensa de heróis na porta? Na Lição 1.6, vamos aprender a automatizar o trabalho com **"Enquanto" e "Para"**!
