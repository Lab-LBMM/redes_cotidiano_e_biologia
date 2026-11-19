# Gosto ou odeio?

Rede bipartida da turma: alunos × disciplinas

1\. Adicionar alunos

Separe vários nomes por vírgula.

2\. Adicionar disciplinas

3\. Criar relações

Nomes novos viram nós automaticamente. Se a dupla já existe, a relação é atualizada.

[ ] **Modo conectar:** toque num aluno e depois numa disciplina (ou vice-versa) na rede

Editar

Clique duplo num nó para renomear; clique duplo numa aresta para trocar gosta ↔ odeia. Arraste os nós para reposicionar. Shift+arrastar seleciona vários. Del exclui, Ctrl+Z desfaz.

Importar arquivo

**Arraste um arquivo aqui**\
ou clique para escolher\
.csv, .tsv, .txt ou .json

…ou colar o texto

Formatos aceitos

**Lista de relações** (uma linha por par). Separador: vírgula, ponto e vírgula ou tabulação.

```
aluno;disciplina;relacao
Ana;Matemática;gosta
Ana;História;odeia
Bruno;Matemática;odeia
```

**Matriz** (alunos nas linhas, disciplinas nas colunas). Use **1**/gosta, **-1**/odeia e **0** ou vazio para nenhuma relação.

```
aluno,Matemática,História,Artes
Ana,1,-1,
Bruno,-1,0,1
```

Também valem *gosto/odeio, like/hate, +/−, sim/não*. Linhas começando com # são ignoradas. Planilhas do Excel/Sheets: salve como CSV. O **JSON** exportado aqui guarda a rede, as posições e a aparência.

Exportar

[ ] PNG com fundo transparente

### Layout

Tipo Orientação Ordem Espaçamento

[ ] Reorganizar ao adicionar nós

### Temas prontos

### Nós: alunos

Cor

Forma Tamanho

### Nós: disciplinas

Cor

Forma Tamanho

[ ] Tamanho proporcional ao nº de conexões (grau)

### Arestas: ♥ gosta

Cor

Traço Espessura

[ ] Mostrar

### Arestas: ✕ odeia

Cor

Traço Espessura

[ ] Mostrar

### Arestas: geral

Curva Opacidade

Rótulo

### Rótulos e fundo

Mostrar nomes

[ ]

Posição Fonte

Cor do texto

Fundo

[ ] Destacar vizinhos ao clicar num nó [ ] Mostrar legenda

Disciplinas

| Disciplina | ♥ | ✕ | Saldo |  |
| --- | --- | --- | --- | --- |

Alunos

| Aluno | ♥ | ✕ | Saldo |  |
| --- | --- | --- | --- | --- |

### Projeção da rede bipartida

Transforma a rede de dois tipos de nós numa rede de um tipo só: dois alunos ficam ligados quando têm a mesma opinião sobre uma disciplina (ou duas disciplinas, quando o mesmo aluno tem a mesma opinião sobre ambas).

O que estou vendo?

Numa **rede bipartida** existem dois conjuntos de nós (alunos e disciplinas) e as arestas só ligam nós de conjuntos diferentes: nunca aluno–aluno nem disciplina–disciplina. As arestas aqui não têm direção e possuem um **sinal**: gosta (+) ou odeia (−).

**Grau** é o número de arestas de um nó. **Saldo** = gosta − odeia. **Densidade** = arestas existentes ÷ arestas possíveis (alunos × disciplinas).

**Sua rede está vazia**Adicione alunos, disciplinas e relações na aba *Construir*, importe um arquivo ou carregue o exemplo.

## Projeção

Ligar quando Peso mínimo 1