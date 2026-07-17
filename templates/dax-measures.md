# Medidas DAX — modelos prontos

Copie e ajuste os nomes de tabela/coluna para o seu esquema estrela (ver `02-fluxo-de-trabalho/3-modelagem-estrela.md`).

```DAX
Total Registros = COUNTROWS('Fato')

Total Valor = SUM('Fato'[Valor])

Média Mensal = AVERAGEX(VALUES('Calendario'[Mês]), [Total Valor])

Variação % MoM =
VAR Atual = [Total Valor]
VAR Anterior = CALCULATE([Total Valor], DATEADD('Calendario'[Data], -1, MONTH))
RETURN DIVIDE(Atual - Anterior, Anterior)

% do Total =
DIVIDE([Total Valor], CALCULATE([Total Valor], ALL('Fato')))
```

## Exemplos aplicados a RH/administrativo

```DAX
Headcount Ativo = CALCULATE(COUNTROWS('Fato_Colaboradores'), 'Fato_Colaboradores'[Status] = "Ativo")

Taxa de Absenteísmo = DIVIDE(SUM('Fato_Ausencias'[Dias]), SUM('Fato_Jornada'[Dias_Uteis]))

Turnover Mensal = DIVIDE([Desligamentos no Mês], [Headcount Início do Mês])
```
