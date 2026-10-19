# As Gavetas do Balcão: O que são Variáveis?
> **Uma Aventura Python** — Por Aya Nicodemos (Ayasoft Studios)  
> *Módulo 1: O Primeiro Dia no Balcão — Lição 3*

---

Atrás do balcão do nosso Empório, a parede é completamente forrada por um enorme móvel de madeira maciça, repleto de pequenas gavetas com puxadores de latão.

Se você deixasse moedas jogadas em cima da mesa, frascos de poção misturados com pergaminhos e nomes de clientes anotados na palma da mão, em dez minutos a loja estaria num caos absoluto!

Para manter tudo em perfeita ordem, nós usamos as **Variáveis**.

Uma variável nada mais é do que uma **gaveta ou caixinha mágica com uma etiqueta de identificação colada na frente** (tipo a bolsa mágica da Hermione, onde você guarda o que quiser e encontra facilmente quando precisar).

---

### Como funciona a Gaveta do Balcão?

Para usar uma gaveta, você pega uma tira de pergaminho, escreve um nome claro nela e cola na frente da gaveta. Por exemplo:  
🏷️ **`ouro no caixa`**

Dentro dessa gaveta, você coloca o número de moedas iniciais da loja: `100`.

Pronto! A partir desse momento, toda vez que o Golem precisar saber quanto dinheiro temos, ele não precisa contar todas as moedas uma por uma: basta abrir a gaveta com a etiqueta `ouro no caixa`.

E por que ela se chama **variável**?  
Porque o conteúdo guardado lá dentro **varia** ao longo do expediente!
* Quando um clérigo compra uma poção por 20 moedas, abrimos a gaveta e trocamos o valor para `120`.
* Quando o fornecedor de frascos de vidro entrega uma encomenda e cobra 10 moedas, o valor diminui para `110`.

A etiqueta da gaveta continua sendo a mesma (`ouro no caixa`), mas o valor lá dentro acompanha a vida financeira da loja!

---

### Os Tipos de Itens que Guardamos nas Gavetas (Tipos de Dados)

Nem tudo na loja é moeda de ouro. Nós temos pergaminhos com textos, frascos com volumes quebrados e estados de lanternas. Na programação, cada tipo de informação tem sua própria natureza:

#### 1. Números Inteiros e Números Quebrados
Números servem para calcular faturamento, somar estoques e dar trocos.

Eles se dividem em dois grupos principais:
* **Inteiros (`int`):** São números inteiros, sem partes fracionadas. Moedas de ouro e quantidades de poções são sempre inteiros.  
  *Exemplos:* `1`, `10`, `50`, `100`, `0`.
* **Decimais ou Ponto Flutuante (`float`):** São números quebrados com casas decimais, como o peso de um saco de ervas ou um preço especial.  
  *Exemplos:* `1.5`, `12.50`, `0.75`.

> ⚠️ **Regra de Ouro da Aya sobre Números Decimais:**  
> Como as linguagens de programação foram criadas no padrão da língua inglesa, você **deve usar sempre o ponto no lugar da vírgula**. Escreva `12.50` e nunca `12,50`. No computador, a vírgula serve para separar itens em listas, e não para casas decimais!

#### 2. Nomes e Textos (Strings)
Os nomes das poções, as frases ditas pelos clientes e as mensagens da loja são guardados como **Strings** (que significa um colar de letras amarradas uma atrás da outra).
* *Exemplos:* `"Empório Mágico da Aya"`, `"Poção de Cura"`, `"Guerreiro Valente"`, `"Olá, forasteiro!"`.

> 🔒 **O Escudo Protetor das Aspas:**  
> Frases, nomes e palavras **sempre devem estar protegidos entre aspas** (sejam aspas duplas `"` ou simples `'`).  
> As aspas avisam ao Golem: *"Isso aqui é um texto falado por humanos, não tente fazer contas de somar ou dividir com essas palavras!"*.  
> Se você escrever `50` sem aspas, o Golem entende como cinquenta moedas (e consegue fazer contas). Se você escrever `"50"` entre aspas, ele entende apenas como o desenho dos caracteres 5 e 0 num cartaz!

#### 3. Lanternas de Estado: Os Booleanos (Verdadeiro ou Falso)
Os booleanos (`bool`) são o tipo mais simples e elegante do reino. Eles só guardam dois valores possíveis no mundo:
* **`Verdadeiro` (True)**
* **`Falso` (False)**

Pense na lanterna mágica pendurada na entrada da nossa loja:
* Se a lanterna está acesa com cristal brilhante (`Verdadeiro`), a loja está **Aberta**.
* Se a lanterna está apagada (`Falso`), a loja está **Fechada**.

Eles servem para tirar dúvidas rápidas do Golem: *O cliente tem ouro suficiente?* (Verdadeiro ou Falso). *A espada está afiada?* (Verdadeiro ou Falso).

---

### Como organizamos as gavetas na Lógica?

Para facilitar a leitura da mente humana (e você não se sentir confuso), na lógica nós escrevemos com palavras claras em português, sem necessidade de underlines, e com linhas bem espaçadas:

```text
nome da loja = "Empório de Poções da Aya"

quantidade de frascos = 15

preco da pocao = 12.50

loja aberta = Verdadeiro
```

Olhe como fica espaçado, limpo e agradável de ler!

Agora que nossas gavetas já estão etiquetadas e abastecidas, na Lição 1.4 vamos aprender a fazer contas e comparar preços: **os Operadores Matemáticos e Lógicos do Python**!
