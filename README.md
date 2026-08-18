# solvefyfull
estrategia de marketing e lançamento de produto solvefy full
Lançamento Solvefy Full — estrutura de execução
Extraído do deck mestre de 14/08/2026. 75 tarefas, de 18/08 a 31/10.
---
1. O problema antes de qualquer coisa: ninguém tem dono
O deck diz "a definir" em 15 lugares — incluindo os 7 donos de pilar e todos os 7 itens da Fase Zero técnica. A própria página 43 avisa: "Sete donos precisam ser nomeados até 20/08. É a única linha deste deck que não depende de verba nem de produção."
Como hoje é 18/08, isso significa:
A Fase Zero do tráfego venceu hoje (verificar BMs) e vence amanhã (pixel, CAPI, base como público) — sem dono nomeado.
4 das 5 decisões de negócio vencem em 22/08, dentro de 4 dias.
Por isso o CSV usa a coluna Papel em vez de responsável. Nomeie a pessoa de cada papel abaixo e o campo Assignees se resolve numa passada só.
Papel	Tarefas	Nome
Comunidade (P7)	12	
Conteúdo (P2)	12	
Mídia / Tráfego (P3)	10	
Produto / Tech	7	
Liderança / decisão	6	
Produto (oferta e preço)	5	
Imprensa (P1)	5	
Operações / CS	4	
Comercial (997+)	3	
Influência (P4)	3	
Financeiro	2	
Canais (P6)	2	
Jurídico	1	
---
2. Como importar no GitHub Projects
Abra o projeto SOLVEFY FULL — GESTÃO DE PROJETO.
No menu `...` do canto superior direito → Import items (ou "Importar itens").
Suba o `plano-lancamento-solvefy.csv`.
Os campos que você já criou (Status, Prioridade, Tamanho, Data de início, Data prevista) são reconhecidos pelo nome. Dois campos novos são criados na importação:
Papel — a função responsável, para você substituir por nome.
Pilar — os 7 pilares do deck, para agrupar a visão de board.
Depois de importar, crie três visualizações:
Board por Pilar — cada pilar é uma coluna, cada dono vê só a dele.
Roadmap por Data prevista — é aqui que a linha do tempo vira Gantt.
Filtro `Prioridade:Alta` + `Data prevista:<2026-08-25` — o que está queimando esta semana.
> Nota: o campo LEIA-ME do Projects não aceita PDF. Suba o deck no repositório `solvefyfull` e cole o link aqui.
---
3. Caminho crítico
O que está em vermelho no fluxo abaixo é o que trava tudo atrás: sem dono nomeado, a Fase Zero não sai; sem Fase Zero, a Fase 1 de mídia não aprende; sem mídia aprendendo, os 70 mil não enchem; sem os 70 mil, não existe R$ 500 mil de lucro.
```mermaid
graph TD
    A["<b>NOMEAR 7 DONOS</b><br/>até 20/08 · Liderança"]:::urgente
    B["<b>FASE ZERO TÉCNICA</b><br/>18 a 21/08 · Mídia + Tech<br/>BMs, pixel, CAPI, UTM, OG, teste CPL"]:::urgente
    C["<b>5 DECISÕES DE OFERTA</b><br/>até 22/08 · Produto + Financeiro<br/>matriz, carteira, antecipação"]:::urgente
    D["Jurídico valida opt-in e LGPD<br/>até 22/08 · Jurídico"]:::urgente
    E["Adquirente, PIX e retry<br/>até 22/08 · Financeiro + Tech"]

    F["Fase 1 de mídia · aquecer<br/>18/08 a 14/09 · 20% da verba"]
    G["Checkout self-service<br/>até 05/09 · Produto"]
    H["100 parceiros mapeados e fechados<br/>25/08 a 15/09 · Influência"]
    I["3 ondas de SMS<br/>25/08 · 08/09 · 15/09 · Comunidade"]
    J["78 grupos abertos<br/>01/09 · Comunidade"]
    K["6 cases gravados + aulas 1 e 2<br/>25/08 a 14/09 · Conteúdo"]

    L["Fase 2 de mídia · captar<br/>15/09 a 30/09 · 45% da verba<br/>CPL teto R$ 6"]
    M["<b>CHECKPOINT 15/09</b><br/>35 mil nos grupos"]:::portao
    N["Oferta congelada + inscrição aberta<br/>15/09 · Produto + Conteúdo"]
    O["Release com embargo<br/>15/09 → publica 22/09 · Imprensa"]

    P["<b>CHECKPOINT 22/09</b><br/>52 mil nos grupos<br/>abaixo de 45 mil = Plano B"]:::portao
    Q["Ep. 6 revela · 27/09<br/>Aulas 1 e 2 no ar · 28 e 29/09"]
    R["9 toques de presença<br/>28/09 a 01/10 · Comunidade"]

    S["<b>LIVE ÚNICA · 01/10, 20h</b><br/>revelação + abertura da oferta<br/>meta 21 mil presentes"]:::marco
    T["Janela de venda · 01 a 10/10<br/>cupom por origem + 1 objeção por dia<br/>Fase 3 de mídia · 35%"]
    U["<b>CORTE 04/10</b><br/>abaixo de 700 vendas = Plano C"]:::portao
    V["<b>META</b><br/>1.750 clientes · R$ 695 mil<br/>R$ 500 mil de lucro"]:::marco
    W["Ativação 80% em 72h<br/>01 a 31/10 · Operações"]:::marco

    A --> B & C & D
    C --> E
    B --> F
    C --> G
    A --> H & I & K
    D --> I
    I --> J
    H --> J
    F --> L
    J --> M
    G --> N
    C --> N
    M --> L
    N --> L
    L --> P
    O --> P
    K --> Q
    P --> Q
    Q --> R
    R --> S
    E --> T
    S --> T
    T --> U
    U --> V
    V --> W

    classDef urgente fill:#3d0000,stroke:#ff4444,stroke-width:2px,color:#fff
    classDef portao fill:#3d3000,stroke:#ffcc00,stroke-width:2px,color:#fff
    classDef marco fill:#003d1a,stroke:#00e676,stroke-width:2px,color:#fff
```
---
4. Os quatro portões numéricos
Não são reuniões de status. Cada um tem número e consequência automática.
Data	Número	Se não bater
15/09	35.000 nos grupos	Libera reserva de mídia de R$ 50–60 mil
22/09	52.000 nos grupos	Abaixo de 45 mil ativa o Plano B: upsell para 997 e 2.997 + Produtora
04/10	700 vendas	Ativa o Plano C: antecipação como oferta ativa do checkout
04/11	80% ativados em 72h	É o indicador que prevê o churn de janeiro
---
5. Duas correções que o deck pede e ainda não têm tarefa
Página 08 vs. página 43: a matriz de planos inclui o degrau de R$ 2.997 (criado na revisão de 15/08), mas a tabela de metas por pilar não menciona o dono dele. O dono comercial nomeado em 20/08 precisa absorver a meta de 30 contratos no 2.997.
Página 17: as datas de roadmap (nov/26, dez/26, 1T/27) estão marcadas como proposta e precisam de validação de produto antes de irem a público — mas a objeção "falta a função X" tem peça marcada para 03/10 e depende delas. A validação precisa sair antes de 22/08, não depois.
