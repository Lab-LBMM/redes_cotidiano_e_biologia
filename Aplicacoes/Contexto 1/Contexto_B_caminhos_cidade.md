# Caminhos da *cidade*

Mapas como redes: locais, ruas e o caminho mais curto

Ferramentas

Criar rua pelo formulário

De Até

Locais novos digitados aqui são criados sem posição no mapa (aparecem no centro).

Ajuda do mapa [ ] O mapa sugere nome, tipo e sentido da rua [ ] O mapa sugere também a distância (modo professor) [ ] Marcar no mapa os locais que ainda faltam

Mapa de fundo

Mapa Imagem

Escala

metros por pixel

Opacidade

[ ] Quadrícula de 100 m [ ] Nomes das ruas no mapa

Para descobrir a escala: meça com a régua algo de tamanho conhecido na imagem (ex.: a barra de escala do mapa) e ajuste os metros por pixel.

Editar

Clique num local ou rua para ver e editar seus **atributos**. Del exclui, Ctrl+Z desfaz, Esc cancela.

Como você vai?

Saindo de Chegando em

Passando por (opcional) O que é “mais curto”?

[ ] 🚦 Horário de pico (avenidas congestionadas para carros)

Anotações do algoritmo

| Local | Melhor valor | Veio de | Situação |
| --- | --- | --- | --- |

Casos para explorar

Como o computador encontra o caminho mais curto?

O método mais usado é o **algoritmo de Dijkstra** (1959). **Algoritmo** é uma sequência de passos bem definidos que sempre leva a uma resposta:

1. Anote **0** na origem e **∞** (infinito, “ainda não sei”) em todos os outros locais.
2. Entre os locais ainda não visitados, escolha o de **menor valor** anotado. Marque-o como **visitado**: esse valor já é o melhor possível.
3. Para cada rua que sai dele **e que pode ser usada no modo escolhido**, some o valor dele ao comprimento da rua. Se der menos do que o anotado no vizinho, troque a anotação e escreva “veio de” este local.
4. Repita os passos 2 e 3 até visitar o destino.
5. Para montar o caminho, volte do destino seguindo as anotações “veio de” até a origem.

Com o critério *menos trechos de rua*, cada rua vale 1 e o algoritmo vira uma **busca em largura**. Com *menor tempo*, cada rua vale o tempo para percorrê-la naquele modo.

Graus dos locais

Conceitos

Vértice (nó)

Cada local da cidade: escola, praça, esquina… Seus **atributos** são nome e tipo.

Aresta

Cada trecho de rua que liga dois locais. Atributos: nome da rua, distância (o **peso** da aresta), tipo de via e sentido.

Grau

Número de arestas ligadas a um vértice. Numa rede direcionada separamos o **grau de entrada** (ruas por onde se chega) e o **grau de saída** (ruas por onde se sai).

Hub

Vértice com muito mais conexões do que os outros: um ponto central da cidade.

Rede não direcionada

As arestas valem nos dois sentidos (a pé, toda rua é de mão dupla).

Rede direcionada

Algumas arestas têm sentido (seta): de carro, uma rua de mão única só pode ser usada numa direção. Por isso a ida pode ser diferente da volta.

Caminho

Sequência de vértices ligados por arestas. O **caminho mais curto** é o de menor soma dos pesos.

### Layout

Posições

Nos layouts abstratos o mapa some: a rede guarda só *quem se liga a quem* e as distâncias, como num mapa de metrô.

### Temas prontos

### Locais (vértices)

Tamanho

Rótulo Fonte

[ ] Tamanho proporcional ao grau [ ] Ícones dentro dos locais [ ] Mostrar nomes das esquinas [ ] Destacar o hub

### Ruas (arestas)

Rótulo Espessura

Ruas

Avenidas

Só pedestres

Caminho

Proibidas no modo

### Fundo e legenda

Fundo

Texto

[ ] Mostrar legenda

Importar

**Arraste um arquivo aqui**\
ou clique para escolher\
.csv, .tsv, .txt ou .json

Formatos aceitos

**Ruas** (uma linha por trecho):

```
origem,destino,rua,distancia,via,sentido
Escola Estadual,Ginásio de Esportes,Rua do Parque,280,rua,dupla
Prefeitura,Padaria Pão Quente,Rua do Comércio,220,rua,unica
```

*via*: rua, avenida, ponte, calcadao, passarela, escadaria, trilha. *sentido*: dupla ou unica (mão única vale de *origem* para *destino*). Colunas opcionais: ciclovia, ladeira (sim/não).

**Locais**: `nome,tipo` (+ `x,y` opcionais). Tipos: escola, saude, comercio, servico, lazer, cultura, transporte, casa, esquina, outro. Nomes iguais aos da cidade fictícia ganham a posição do mapa.

Exportar

**Algoritmo**

local atualvisitado (valor definitivo)valor provisóriorua sendo examinada“veio de”

**Bem-vindo a Vila Esperança!**

Observe o mapa: encontre os locais importantes (inclusive a **escola**) e as ruas que os ligam. Depois construa a **rede**: cada local vira um vértice e cada trecho de rua, uma aresta com nome e distância.