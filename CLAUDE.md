# Contexto do projeto

Este repositório é um roteiro de aprendizado para construir dashboards em Power BI a partir de dados administrativos/RH, do zero até a publicação — para ser seguido com apoio do Claude Code.

## Como agir ao ajudar quem está usando este repositório

- A pessoa está aprendendo o fluxo; explique o "porquê" de cada etapa antes do "como", sem pressupor conhecimento avançado de dados ou Power BI.
- Siga a ordem dos arquivos em `02-fluxo-de-trabalho/` como roteiro principal — são etapas sequenciais, não peça para pular para o dashboard sem antes tratar e modelar os dados.
- Adapte os exemplos ao caso real dela (folha de pagamento, headcount, absenteísmo, turnover, admissões/desligamentos etc.), mesmo que os arquivos tragam exemplos genéricos.
- Quando surgir uma medida ou cálculo reutilizável, sugira registrar em `templates/dax-measures.md` para virar referência permanente.
- Ao revisar um problema (dado errado, medida que não bate, visual confuso), aponte em qual etapa do fluxo (`01` a `05`) o problema provavelmente se originou.
- Ver `03-trabalho-conjunto/colaboracao-e-revisao.md` para como registrar dúvidas e pedir revisão de volta.

## Estrutura

```
01-fundamentos/            → o que é cada ferramenta usada e para que serve
02-fluxo-de-trabalho/      → etapas, em ordem: entrada → tratamento → modelagem → medidas → dashboard
03-trabalho-conjunto/      → como pedir ajuda, registrar dúvidas, revisar junto
templates/                 → modelos prontos para copiar e adaptar
```
