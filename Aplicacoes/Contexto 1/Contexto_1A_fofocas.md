# Por onde a notícia *passou?*

Mapa de percolação de uma informação na escola

Registrar a resposta de um aluno

Nome * Sala

Quem te contou? Para quem você contou?

Como ficou sabendo? Que horas?

[ ] É **semente** (recebeu a notícia da equipe) [ ] Não ficou sabendo da notícia

Nomes novos viram nós. Se dois relatos descrevem a mesma passagem (A diz que contou para B e B diz que ouviu de A), ela fica **confirmada**.

Ligação direta

→

[ ] **Modo conectar:** toque em quem contou e depois em quem ouviu

Salas da escola

Cadastre todas as salas, inclusive as que talvez não recebam a notícia: assim o mapa mostra onde ela *não* chegou.

Editar

Clique num aluno para ver o **caminho** da notícia até ele e a **cascata** que ele gerou. Clique duplo para renomear. Para unir dois nomes do mesmo aluno (ex.: “João” e “João P.”), selecione os dois com Shift e use *Juntar*. Del exclui, Ctrl+Z desfaz.

Importar arquivo

**Arraste um arquivo aqui**\
ou clique para escolher\
.csv, .tsv, .txt ou .json (inclusive a exportação do Google Formulários)

Dica: importe primeiro a **lista de alunos** da escola e depois as respostas: quem não aparece em nenhuma passagem fica marcado como “não soube”.

…ou colar o texto

Formatos aceitos

**1. Respostas** (uma linha por aluno entrevistado). Vários nomes em “para quem” separados por **;** ou **|** (ou vírgula, se o separador do arquivo for ;).

```
nome,sala,quem_te_contou,para_quem_contou,meio,hora
Ana,7A,equipe,Bruno;Carla,Pessoalmente,07:30
Bruno,7A,Ana,Diego,WhatsApp,08:10
Diego,8B,Bruno,,Pessoalmente,08:40
Elisa,9A,,,,
```

Se “quem te contou” for *equipe, professor(a), direção* ou *pesquisa*, o aluno vira **semente**. Uma coluna *soube* (sim/não) ou *semente* (sim) também é reconhecida.

**2. Lista de passagens** (uma linha por “A contou para B”):

```
de,sala_de,para,sala_para,hora,meio
Ana,7A,Bruno,7A,08:10,WhatsApp
```

**3. Lista de alunos** (para saber quem não recebeu): `nome,sala` (+ `semente` opcional).

O **JSON** exportado aqui restaura tudo: rede, posições e aparência. Planilhas do Excel/Sheets: salve como CSV.

Perguntas sugeridas para um formulário

```
1. Seu nome
2. Sua sala (turma)
3. Você ficou sabendo da notícia? (sim/não)
4. Quem te contou?
5. Como você ficou sabendo? (pessoalmente,
   WhatsApp, Instagram, outro)
6. Mais ou menos que horas?
7. Para quem você contou? (nomes separados
   por vírgula)
```

Com essas perguntas, o CSV exportado do Google Formulários pode ser importado direto: as colunas são reconhecidas pelo texto das perguntas.

Exportar

[ ] PNG com fundo transparente

Modelos para preencher

### Layout

Tipo Espaçamento

[ ] Mostrar quem não soube [ ] Reorganizar ao adicionar alunos

### Temas prontos

### Cor dos alunos

Colorir por

Sementes

Última geração

Poucos

Muitos

Cor

Contorno da semente

Não souberam

### Forma e tamanho

Forma Forma da semente Tamanho por Tamanho base

### Setas (passagens)

Cor Cor única

Espessura

Ponta da seta

Curva Rótulo

[ ] Destacar passagens entre salas

Cor das pontes

[ ] Tracejar passagens não confirmadas (só um lado relatou)

### Rótulos e fundo

Mostrar nomes

[ ]

Fonte

Cor do texto

Fundo

[ ] Ao clicar, destacar caminho e cascata [ ] Mostrar legenda

Salas

| Sala | Souberam |  | Chegou | Vinda de fora |
| --- | --- | --- | --- | --- |

Quem mais repassou

| Aluno | Sala | Contou p/ | Alcance | Pontes |
| --- | --- | --- | --- | --- |

Sementes

| Semente | Sala | Cascata | Salas | Gerações |
| --- | --- | --- | --- | --- |

O que é percolação?

**Percolação** é o estudo de quando algo consegue atravessar um meio: a água pelo pó de café, uma doença por uma população, uma notícia por uma escola. Cada passagem de um aluno a outro é um “poro” aberto. Se existem caminhos suficientes, a informação *percola* e chega a quase todas as salas; se há poucos, ela fica presa em grupos isolados.

**Geração**: quantos passos a notícia levou desde as sementes. **Alcance**: quantas pessoas ficaram sabendo “descendo” a partir de um aluno. **Pontes**: passagens entre salas diferentes, essenciais para a notícia sair do grupo de origem. **Confirmada**: quem contou e quem ouviu relataram a mesma passagem.

**Nenhum dado ainda**Cadastre as salas, registre as respostas dos alunos na aba *Construir*, importe um arquivo ou carregue o exemplo.

## Rede de salas

Layout [x] Mostrar salas não alcançadas