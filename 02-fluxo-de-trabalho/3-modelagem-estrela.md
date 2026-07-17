# 3. Modelagem (esquema estrela)

O Power BI funciona melhor — mais rápido e com DAX mais simples — quando os dados são organizados em **esquema estrela**: uma tabela fato (os eventos/registros) cercada de tabelas dimensão (os "recortes" pelos quais você quer analisar).

## Estrutura genérica

```
        Dim_Calendario
              |
Dim_Departamento — Fato_Registros — Dim_Colaborador
              |
        Dim_Centro_de_Custo
```

- **Fato_Registros**: uma linha por evento (ex.: um pagamento, um dia de ausência, uma admissão) + valores numéricos (valor, horas, dias)
- **Dim_Calendario**: uma linha por dia/mês, para filtrar e comparar períodos
- **Dim_Departamento / Dim_Colaborador / Dim_Centro_de_Custo**: uma linha por item único, com os atributos que descrevem esse item

## Regra prática

Se uma informação **se repete** em várias linhas da fato (nome do departamento, cargo, gestor), ela pertence a uma dimensão — não à tabela fato.

## Pergunta para levar ao Claude Code

"Com base na minha base tratada, como ficaria a fato e as dimensões desse esquema estrela?"

Próxima etapa: `4-medidas-dax.md`
