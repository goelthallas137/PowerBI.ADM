# 2. Tratamento e limpeza

Objetivo: sair com uma base confiável, sem precisar "confiar no acaso" nos números depois.

## Checklist de limpeza

- **Duplicados** — mesmo colaborador/registro aparecendo mais de uma vez sem motivo
- **Nulos** — decidir, campo a campo, se um vazio significa "zero", "não se aplica" ou "erro de preenchimento" (nunca assumir automaticamente)
- **Padronização de categorias** — "RH", "Rh", "recursos humanos" devem virar um único valor
- **Datas** — formato único (ex.: AAAA-MM-DD), sem texto misturado
- **Valores numéricos** — sem separador de milhar como texto, sem símbolo de moeda dentro da célula
- **Outliers óbvios** — um salário digitado com um zero a mais, uma data de admissão no futuro

## Por que isso importa antes de modelar

Um erro de limpeza não tratado vira um número errado no dashboard final — e nesse ponto fica muito mais difícil de rastrear a origem.

## Pergunta para levar ao Claude Code

"Depois de aplicar essa checklist na minha base de [assunto], quais problemas você encontrou e como sugere resolver cada um?"

Próxima etapa: `3-modelagem-estrela.md`
