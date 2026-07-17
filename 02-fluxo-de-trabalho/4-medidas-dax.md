# 4. Medidas DAX

Medida é um cálculo que responde a uma pergunta de negócio e se adapta automaticamente aos filtros do dashboard (período, departamento, etc.) — diferente de uma coluna calculada, que é fixa linha a linha.

## Perguntas de negócio → medida

| Pergunta | Vira medida |
|---|---|
| "Quantos registros temos no total?" | Contagem simples |
| "Qual o valor total no período filtrado?" | Soma condicionada ao filtro |
| "Como está esse mês comparado ao anterior?" | Comparação com período anterior |
| "Que fatia esse departamento representa do total?" | Percentual sobre o total geral |

Os modelos prontos para essas quatro perguntas estão em `templates/dax-measures.md` — copie e troque os nomes de tabela/coluna pelos da sua base.

## Regra prática

Se você está tentado a criar uma **coluna** para responder algo que muda com o filtro (mês, departamento), quase sempre o certo é uma **medida**.

## Pergunta para levar ao Claude Code

"Baseado no meu esquema estrela, quais medidas eu preciso para responder [pergunta de negócio]?"

Próxima etapa: `5-dashboard-e-publicacao.md`
