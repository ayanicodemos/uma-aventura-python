# Dias de Feira Movimentada: Repetições com "Enquanto" e "Para"
> **Uma Aventura Python** — Por Aya Nicodemos (Ayasoft Studios)  
> *Módulo 1: O Primeiro Dia no Balcão — Lição 6*

---

Chegamos à última e mais empolgante lição do nosso primeiro módulo! 

Você já sabe registrar preços nas gavetas, calcular faturamentos com os operadores e tomar decisões inteligentes com o "Se".

Agora, imagine o seguinte dia de glória no nosso Empório:

> *A guilda inteira de aventureiros acabou de voltar vitoriosa de uma incursão ao calabouço. Quando você abre as portas da loja às oito da manhã, há uma fila de **100 aventureiros sedentos por poções** esperando na calçada!*

Você vai escrever o código de atender, cobrar e entregar o frasco 100 vezes seguidas no seu bloco de notas?
* *Atende guerreiro 1...*
* *Atende arqueira 2...*
* *Atende clérigo 3...*
* *(...) até o herói número 100?!*

De jeito nenhum! Ninguém aguenta esse trabalho monótono. 

Nós, seres humanos, nos cansamos, ficamos com sono, nos distraímos e começamos a errar o troco quando fazemos a mesma tarefa dezenas de vezes. Mas adivinhe só quem **ama** tarefas repetitivas e tem energia infinita para trabalhar o dia todo sem reclamar? **O nosso Golem de pedra!**

Para colocar o Golem para trabalhar no piloto automático, usamos as **Estruturas de Repetição** (conhecidas pelos programadores como **Laços** ou **Loops**).

Existem duas estruturas principais que você precisa dominar: o **"Enquanto"** e o **"Para"**.

---

### 1. A Estrutura "Enquanto" (While)

A estrutura **"Enquanto"** funciona monitorando uma condição no balcão. Ela diz ao Golem:  
> *"Continue repetindo este bloco de instruções **ENQUANTO** esta condição continuar sendo Verdadeira!"*

Veja como automatizamos a fila da loja, com passos bem espaçados para respirar:

```text
clientes na fila = 10



ENQUANTO (clientes na fila > 0):

    DIZER: "Próximo aventureiro, por favor!"
    
    ATENDER: pedido do heroi
    
    ENTREGAR: pocao comprada
    
    clientes na fila = clientes na fila - 1



DIZER: "Ufa! A fila acabou. Hora de fechar as portas e contar o ouro do dia!"
```

Veja como o Golem executa:
1. Começa com 10 clientes. 10 é maior que 0? **Sim!** Atende o primeiro e diminui para 9.
2. Tem 9 clientes. 9 é maior que 0? **Sim!** Atende o segundo e diminui para 8.
3. (...)
4. Quando restar 1 cliente, ele atende com capricho e diminui para 0.
5. O Golem volta ao topo e pergunta: *0 é maior que 0?* **Não!** A condição virou Falsa!
6. O Golem sai da repetição e anuncia que a fila acabou com sucesso.

#### ⚠️ O Perigo do "Loop Infinito":
O que aconteceria se você esquecesse de colocar a linha que diminui a fila (`clientes na fila = clientes na fila - 1`)?  
A fila continuaria para sempre com 10 clientes, e o Golem continuaria atendendo fantasmas sem parar até as engrenagens de pedra dele esquentarem e quebrarem! Sempre garanta que em algum momento a sua condição se torne falsa para o programa poder descansar.

---

### 2. A Estrutura "Para" (For)

Enquanto o "Enquanto" depende de uma condição no balcão, a estrutura **"Para"** é usada quando você quer inspecionar uma coleção fechada de itens, um por um, do primeiro até o último frasco.

Imagine que uma caravana de anões comerciantes acabou de descarregar uma caixa de madeira com **5 novas Poções de Mana**. Você precisa colar a etiqueta de preço em cada frasco:

```text
caixa de pocoes = ["Poção Azul", "Poção Verde", "Poção Roxa", "Poção Vermelha", "Poção Dourada"]



PARA CADA pocao NA caixa de pocoes:

    PEGAR: pocao da caixa
    
    LIMPAR: poeira do vidro
    
    COLAR ETIQUETA: "25 moedas de ouro"
    
    COLOCAR: pocao na prateleira da loja



DIZER: "Todas as poções da caixa foram etiquetadas e guardadas na vitrine!"
```

Veja que elegância: o comando **"Para cada..."** automaticamente pega o primeiro frasco da caixa, executa todos os passos, passa para o segundo, para o terceiro... e quando a caixa fica vazia, ele encerra o trabalho sozinho sem você ter que controlar nenhum número!

---

### 🎉 Parabéns! Você dominou a Lógica do Balcão!

Respire fundo e olhe para trás com orgulho. Em 6 lições completas e acolhedoras, você aprendeu:
1. Como a programação nasceu com Ada Lovelace e Grace Hopper, e como o Golem traduz receitas;
2. Como organizar o atendimento passo a passo com algoritmos impecáveis;
3. Como guardar itens em gavetas e caixinhas mágicas com as variáveis e seus tipos de dados;
4. Como usar os operadores matemáticos e comparadores do Python (`+`, `-`, `*`, `/`, `==`, `!=`, `>`, `<`, `>=`, `<=`, `and`, `or`);
5. Como tomar decisões no balcão com o "Se" (`SE`, `SENÃO SE`, `SENÃO`);
6. Como automatizar filas e caixas de itens com "Enquanto" e "Para".

Você não tem mais apenas vontade de aprender: **você agora pensa como um programador!**

Chegou a hora de provar a sua sabedoria na nossa **Arena de Desafios** abaixo!
