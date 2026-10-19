# Os Operadores Lógicos e Matemáticos
> **Uma Aventura Python** — Por Aya Nicodemos (Ayasoft Studios)  
> *Módulo 1: O Primeiro Dia no Balcão — Lição 4*

---

Na lição anterior, você aprendeu a guardar informações dentro das caixinhas mágicas chamadas variáveis. 

Agora, a pergunta de um milhão de moedas de ouro é: **o que a gente faz com essas informações?**

É aqui que entram os **Operadores**! Eles são os símbolos e ferramentas que você usa para somar valores, calcular trocos, comparar preços e fazer perguntas lógicas para o computador.

Vamos conhecer exatamente os mesmos operadores que o Python utiliza, explicados de forma simples e direta para o balcão da sua loja:

---

### 1. Os Operadores Aritméticos (As Contas do Balcão)

Esses são os responsáveis por fazer as contas matemáticas do dia a dia da sua loja:

| Símbolo | Nome | O que ele faz no balcão da loja? | Exemplo |
| :---: | :--- | :--- | :--- |
| `+` | **Adição** | Soma valores ou junta dois textos | `10 + 5` dá `15` |
| `-` | **Subtração** | Diminui valores ou calcula o troco | `20 - 15` dá `5` |
| `*` | **Multiplicação** | Multiplica quantidades (usa-se o asterisco!) | `3 * 10` dá `30` |
| `/` | **Divisão** | Divide um valor (usa-se a barra inclinada!) | `50 / 2` dá `25.0` |

> 💡 **Repare bem:**  
> No teclado do computador, nós não usamos o "x" para multiplicar nem os "dois pontos com traço ÷" para dividir. Nós usamos o **asterisco `*`** para multiplicar e a **barra `/`** para dividir!

---

### 2. O Grande Duelo: `=` (Guardar) vs. `==` (Comparar)

Aqui está **a pegadinha número 1 de todo mundo que começa a programar**. Preste muita atenção para nunca mais esquecer isso:

* **Um sinal de igual sozinho (`=`): Atribuição.**  
  Significa: *"Pegue esse valor da direita e guarde dentro da caixinha da esquerda!"*.  
  
  ```text
  preco da pocao = 15
  ```

* **Dois sinais de igual juntos (`==`): Comparação de Igualdade.**  
  Significa: *"Ei, computador! O valor da esquerda é exatamente igual ao valor da direita?"*.  
  
  ```text
  senha digitada == "abracadabra"
  ```
  *(O computador responde com Verdadeiro se for igual, ou Falso se for diferente).*

Se você quer guardar, use `=`. Se você quer perguntar se são iguais, use `==`!

---

### 3. Os Operadores Relacionais (As Comparações de Preço)

No balcão, você precisa comparar coisas o tempo todo. Por exemplo: *O dinheiro do cliente dá para pagar a espada?*

Para isso, usamos os operadores relacionais, e a resposta que o computador nos dá é sempre um Booleano (`Verdadeiro` ou `Falso`):

| Símbolo do Python | Significado | Exemplo Prático | Resposta do Computador |
| :---: | :--- | :--- | :---: |
| `>` | **Maior que** | `ouro do cliente > 50` | `Verdadeiro` (se o cliente tiver mais de 50) |
| `<` | **Menor que** | `preco < 10` | `Falso` (se o preço for 15) |
| `>=` | **Maior ou igual a** | `nivel do heroi >= 10` | `Verdadeiro` (se tiver 10 ou mais) |
| `<=` | **Menor ou igual a** | `moedas no bolso <= 20` | `Verdadeiro` (se tiver 20 ou menos) |
| `!=` | **Diferente de** | `classe do heroi != "Ladino"` | `Verdadeiro` (se não for um ladino) |

> 📌 **Dica da Aya:**  
> O símbolo de "diferente de" no computador é escrito com um ponto de exclamação e um igual: `!=`. Pense no ponto de exclamação como um grito de *"NÃO é igual!"*.

---

### 4. Os Conectivos Lógicos: `E`, `OU` e `NÃO` (and, or, not)

Às vezes, uma condição só não basta. Imagine a seguinte regra na sua loja:

> *"Para comprar o Elmo Sagrado, o aventureiro precisa ter **nível 10 ou mais** E precisa ter **pelo menos 100 moedas de ouro**."*

Para juntar duas condições, o Python usa três termos simples:

* **`and` (E):** Exige que **todas** as condições sejam verdadeiras.  
  
  ```text
  nivel do heroi >= 10  and  moedas do heroi >= 100
  ```
  *(Se o guerreiro tiver nível 10, mas só tiver 80 moedas, a resposta é Falso — nada de elmo pra ele!).*

* **`or` (OU):** Exige que **pelo menos uma** das condições seja verdadeira.  
  
  ```text
  classe do heroi == "Mago"  or  tem passe especial == Verdadeiro
  ```

* **`not` (NÃO):** Inverte o valor. Se algo é Verdadeiro, o `not` transforma em Falso.

Agora que você já sabe fazer contas e comparar grandezas, você tem tudo o que precisa para o próximo grande salto: **ensinar o seu Golem a tomar decisões sozinho com o famoso "Se"**!
