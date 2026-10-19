# A Balança e o Caixa: Operadores Matemáticos e Lógicos
> **Uma Aventura Python** — Por Aya Nicodemos (Ayasoft Studios)  
> *Módulo 1: O Primeiro Dia no Balcão — Lição 4*

---

Na lição anterior, você aprendeu a colocar informações nas gavetas da loja. 

Agora vem a pergunta de um milhão de moedas: **como o Golem faz as contas das vendas e confere se os clientes estão pagando o valor certo?**

Para isso, usamos os **Operadores**. Eles são os símbolos matemáticos e lógicos que você digita no teclado para mandar o Golem somar faturamentos, calcular trocos e comparar preços.

No Python, nós usamos exatamente os símbolos abaixo. Vamos conhecê-los com calma:

---

### 1. As Quatro Operações do Caixa (Aritmética)

Para somar moedas, calcular lucros e dividir fardos de poções:

| Símbolo no Teclado | Nome | O que ele faz no caixa da loja? | Exemplo Prático |
| :---: | :--- | :--- | :--- |
| `+` | **Adição** | Soma moedas ou junta duas frases | `10 + 5` resulta em `15` |
| `-` | **Subtração** | Diminui despesas ou calcula o troco | `20 - 15` resulta em `5` |
| `*` | **Multiplicação** | Multiplica o preço pela quantidade | `3 * 10` resulta em `30` |
| `/` | **Divisão** | Divide um fardo de itens | `50 / 2` resulta em `25.0` |

> 💡 **Repare bem no teclado:**  
> Computadores não usam a letra "x" para multiplicar nem a barra com dois pontinhos (÷) para dividir. Nós usamos o **asterisco `*`** para multiplicar e a **barra inclinada `/`** para dividir!

---

### 2. O Grande Duelo: `=` (Guardar) vs. `==` (Comparar)

Aqui está **a pegadinha número 1 de quase todo mundo que começa a programar**. Preste muita atenção para nunca mais errar:

* **Um sinal de igual sozinho (`=`): Atribuição.**  
  Significa: *"Pegue o valor da direita e guarde dentro da gaveta da esquerda!"*.  
  
  ```text
  preco da pocao = 15
  ```
  *(Aqui você está guardando o número 15 dentro da gaveta).*

* **Dois sinais de igual juntos (`==`): Comparação de Igualdade.**  
  Significa: *"Ei, Golem! O que está na esquerda é exatamente igual ao que está na direita?"*.  
  
  ```text
  senha do cofre == "abracadabra"
  ```
  *(O Golem confere e responde: Verdadeiro se for igual, ou Falso se for diferente).*

Se você quer guardar na gaveta, use um igual `=`. Se você quer perguntar se são iguais, use dois iguais `==`!

---

### 3. As Comparações de Preço e Nível (Operadores Relacionais)

No balcão, você precisa comparar grandezas o tempo todo. Por exemplo: *O herói tem ouro suficiente para pagar a espada? O aventureiro tem nível suficiente para empunhar o machado mágico?*

Para isso, usamos os símbolos relacionais digitados diretamente no teclado:

* `>` : **Maior que**  
  *Exemplo:* `ouro do cliente > 50` (Verdadeiro se ele tiver mais de 50 moedas).
* `<` : **Menor que**  
  *Exemplo:* `preco do item < 10` (Verdadeiro se o item for uma pechincha menor que 10).
* `>=` : **Maior ou igual a** *(digita-se o sinal de maior `>` e em seguida o sinal de igual `=`)*  
  *Exemplo:* `nivel do heroi >= 10` (Verdadeiro se tiver nível 10 ou superior).
* `<=` : **Menor ou igual a** *(digita-se o sinal de menor `<` e em seguida o sinal de igual `=`)*  
  *Exemplo:* `peso da mochila <= 30` (Verdadeiro se a mochila pesar 30 quilos ou menos).
* `!=` : **Diferente de** *(digita-se o ponto de exclamação `!` seguido do igual `=`). Pense na exclamação gritando: "NÃO é igual!"*  
  *Exemplo:* `classe do heroi != "Ladino"` (Verdadeiro se o cliente não for um ladino).

> 📌 **Aviso Visual Importante da Aya:**  
> Repare que para escrever "maior ou igual" nós usamos **dois caracteres do teclado juntos**: `>=`. E para "diferente", usamos `!=`. Nunca usamos caracteres desenhados de livros escolares como `⩾` ou `≠`, porque essas teclas não existem no teclado comum do computador!

---

### 4. As Regras da Guilda: `and`, `or` e `not`

Às vezes, uma condição só não é suficiente para fechar negócio. Imagine uma regra especial da guilda de aventureiros na sua loja:

> *"Para comprar o Elmo Sagrado de Mithril, o aventureiro precisa ter **nível 10 ou mais** E precisa ter **pelo menos 100 moedas de ouro**."*

No Python, nós usamos três palavras simples para juntar essas regras:

* **`and` (E):** Exige que **todas** as condições sejam verdadeiras ao mesmo tempo.  
  
  ```text
  nivel do heroi >= 10   and   ouro no bolso >= 100
  ```
  *(Se o herói for nível 20, mas só tiver 80 moedas, a resposta é Falsa: ele não leva o elmo!).*

* **`or` (OU):** Exige que **pelo menos uma** das condições seja verdadeira.  
  
  ```text
  classe do heroi == "Mago"   or   tem passe vip == Verdadeiro
  ```
  *(Se ele for um guerreiro com passe VIP, ele já ganha o atendimento especial!).*

* **`not` (NÃO):** Inverte o resultado. Se algo era Verdadeiro, o `not` faz virar Falso.

Com as contas e comparações dominadas, agora podemos ensinar o Golem a tomar decisões com o **famoso "Se"** na Lição 1.5!
