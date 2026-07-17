# 1. Entrada de dados

Antes de qualquer tratamento, entenda o que está entrando.

## De onde os dados costumam vir

- Exportações de sistemas (folha de pagamento, ponto, ERP) em Excel/CSV
- Planilhas mantidas manualmente por RH/administrativo
- Formulários ou registros consolidados por outra pessoa

## O que checar assim que a planilha chega

1. **Uma linha = um registro?** (ex.: uma linha por colaborador/mês, não por célula solta)
2. **Cabeçalhos claros e únicos** — evite colunas sem nome ou repetidas
3. **Tipos consistentes por coluna** — datas sempre como data, valores sempre como número (não texto com "R$")
4. **Sem células mescladas** — mescla quebra qualquer ferramenta de análise
5. **Uma aba = uma tabela** — se a planilha mistura vários assuntos numa aba só, ela precisa ser separada antes de seguir

## Pergunta para levar ao Claude Code

"Aqui está minha planilha bruta de [assunto] — ela está pronta para tratamento ou tem algo que preciso ajustar antes?"

Próxima etapa: `2-tratamento-e-limpeza.md`
