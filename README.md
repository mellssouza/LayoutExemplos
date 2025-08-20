1. FrameLayout

O que faz:
O FrameLayout é o layout mais simples. Ele posiciona seus elementos empilhados, um em cima do outro, na ordem em que são declarados.

Quando usar:
Quando você quer colocar um elemento sobre o outro, tipo uma imagem de fundo e texto por cima, ou um layout simples que não precisa de muitas regras de posicionamento.

Exemplo explicado:
No exemplo, a imagem ocupa toda a tela (fundo) e o texto fica centralizado em cima dela usando android:layout_gravity="center".



2. LinearLayout

O que faz:
Organiza os elementos em sequência, podendo ser na vertical ou horizontal.

Quando usar:
Para layouts simples que você quer alinhar itens em uma coluna ou linha, tipo uma lista curta de botões ou textos.

Exemplo explicado:
Os elementos são colocados um embaixo do outro (orientation="vertical"), o TextView fica em cima e o Button embaixo.



3. RelativeLayout

O que faz:
Posiciona os elementos com base em suas relações, como “abaixo de”, “à direita de” ou “alinhado ao centro do pai”.

Quando usar:
Para layouts onde os elementos precisam ficar posicionados em relação uns aos outros, mas você não quer usar um LinearLayout com vários aninhamentos.

Exemplo explicado:
O botão fica posicionado logo abaixo do campo de texto com margem, usando android:layout_below="@id/campoTexto".



4. ConstraintLayout

O que faz:
É um layout muito poderoso que permite posicionar elementos com restrições em relação a outros elementos ou ao pai, sem necessidade de aninhamento pesado.

Quando usar:
Para layouts complexos que precisam ser flexíveis e performáticos, evitando hierarquias profundas. É o layout mais recomendado para interfaces modernas.

Exemplo explicado:
O texto está posicionado no topo da tela, centralizado horizontalmente, por meio das restrições layout_constraintStart_toStartOf="parent" e layout_constraintEnd_toEndOf="parent", com uma margem no topo.



5. RecyclerView

O que faz:
Exibe uma lista grande de itens de forma eficiente, reutilizando as views que saem da tela para economizar memória e melhorar performance.

Quando usar:
Sempre que precisar mostrar listas ou grids que podem crescer dinamicamente, como listas de contatos, produtos, mensagens etc.

Como funciona:
O RecyclerView é configurado com um Adapter que cria e “recicla” os itens conforme o usuário rola a lista. No XML, você só coloca o RecyclerView, e o resto é feito em código.

Exemplo explicado:
O XML define onde a lista aparece, e o item de layout define a aparência de cada linha (ex: um TextView). O Adapter manipula a lógica para preencher e reutilizar esses itens.
