# Roteiro — Apresentação Rápida do Dashboard de Vendas

**Duração alvo:** ~5 minutos · **Formato:** Power BI Desktop aberto ao vivo, navegando Executiva → Produtos
**Antes de começar:** deixe o filtro de Mês/Ano no período mais recente com dado fechado.

---

## 0. A pergunta que o dashboard responde (mentalize antes de abrir a boca)

> "Tablets lidera a receita — mas essa liderança se traduz em lucro?"

Essa é a hipótese central do projeto inteiro. Toda a apresentação é a resposta a essa pergunta, em 3 atos: Executiva mostra o sintoma, Produtos mostra a causa, a tabela mostra o culpado exato.

---

## 1. Abertura (30s)

> "Esse é um dashboard de vendas de uma distribuidora de eletrônicos. A pergunta que ele responde não é 'quem vende mais' — isso todo mundo já sabe. É 'quem vende mais **e** dá mais lucro' — e a resposta tem uma pegadinha."

---

## 2. Página Executiva — o farol (1 min)

**O que está na tela:** 4 KPIs no topo (% Atingimento · Faturamento Total · Meta Total · % Margem), um combo de Faturamento vs. Meta por mês, e um ranking de % Margem por categoria.

> "Aqui em cima estão os 4 números que uma Diretora Comercial quer ver primeiro: se batemos a meta, quanto faturamos, qual era a meta, e qual a margem. [aponte o gráfico de barras à direita] Esse ranking já entrega a primeira pista: reparem que a categoria com a barra mais curta de margem é justamente uma das que mais fatura. Vamos entender por quê na próxima página."

---

## 3. Página Produtos — o coração da história (2 min)

**O que está na tela:** 3 KPIs (Faturamento Total · % Margem · Categoria Líder em Receita), no meio um gráfico de dispersão (Faturamento × % Margem por categoria) + uma barra de alerta, embaixo a tabela de ranking de produtos com classificação de margem.

> "Aqui é onde a história fecha. [aponte o gráfico de dispersão] No eixo horizontal está quem vende mais; no vertical, quem tem mais margem. Reparem que **Tablets** está lá embaixo à direita — é a categoria que mais fatura, mas tem a **pior margem** de todas: 30%, contra 50% de Áudio, que fatura menos mas é a mais lucrativa. [aponte a barra vermelha] Essa cor não é decoração — ela já entrega o alerta antes de eu precisar explicar. [aponte a tabela] E descendo pro detalhe produto a produto: os dois produtos que mais faturam da empresa inteira — Tab Max 12 e Tab Pro 11 — são justamente os dois com classificação 'Baixa' margem. Não é a categoria em abstrato: são produtos específicos, com nome, puxando o resultado pra baixo."

---

## 4. A métrica que confunde todo mundo: **p.p.** (1 min — explicação dedicada)

Esse é o ponto em que vale parar e explicar, porque é onde a audiência mais trava.

**O que é:** "p.p." = **pontos percentuais**. É a diferença simples entre dois percentuais — não uma variação relativa.

**Use o próprio card de % Margem como exemplo ao vivo:**

> "Vejam esse card: % Margem está em 39,17%, e embaixo aparece '▼ 0,83 p.p. vs meta (40%)'. Isso significa uma coisa muito simples: `39,17 − 40 = −0,83`. É a **subtração direta** entre os dois percentuais — não é dizer que a margem caiu 0,83% em relação à meta, que seria outra conta e outro número."

**Por que não usar "%" aqui — o exemplo que gruda na cabeça:**

> "Se a margem fosse de 10% e subisse pra 20%, dá pra descrever de duas formas bem diferentes: subiu **10 pontos percentuais** (a conta direta, `20 − 10`), ou subiu **100% em termos relativos** (dobrou). Os dois números estão certos — descrevem coisas diferentes. Quando estamos comparando **percentual com percentual** — como margem atual vs. meta de margem, ou participação de uma categoria mês a mês — a pergunta certa é 'quantos pontos percentuais mudou', não 'quantos por cento mudou'. Por isso o dashboard usa p.p. nesses casos: evita a armadilha de fazer 'percentual do percentual'."

**Regra de bolso pra fixar:** valor absoluto (R$) comparado com valor absoluto → **%** relativo faz sentido (ex.: Faturamento subiu 11% vs. mês anterior). Percentual comparado com percentual → **p.p.**, sempre.

---

## 5. Fechamento (30s)

> "Resumindo: Tablets é o motor de receita da empresa, mas também é onde a margem está sendo sacrificada — e a página de Produtos existe justamente pra deixar isso visível numa olhada só, sem precisar abrir planilha nenhuma."

**Nota honesta pra você (não fala isso pra audiência a não ser que perguntem):** a página **Vendedores** ainda é só a casca de navegação — sem visuais de conteúdo ainda. Se alguém clicar nela, tenha uma frase pronta: *"essa página é o próximo passo do projeto, ainda em construção."* Não force uma demonstração do que não existe.

---

## Perguntas prováveis e respostas curtas

- **"Por que Tablets tem margem tão baixa?"** → é o dado de custo da categoria (não investigamos causa raiz nesta fase — é uma pergunta de próxima etapa, não deste dashboard).
- **"Dá pra ver isso por vendedor?"** → ainda não, está na página Vendedores, em construção.
- **"O 'mês atual' muda sozinho?"** → sim, o card sempre pega o mês mais recente com dado, filtrado pelos slicers de Mês/Ano no topo — não é fixo.
