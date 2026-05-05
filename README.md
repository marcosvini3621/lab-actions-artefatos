# Pipeline Inteligente com Artefatos

## Objetivo

Criar um workflow otimizado que roda apenas quando necessário e armazena arquivos gerados utilizando artefatos.

## Funcionalidades

* Execução manual (workflow_dispatch)
* Execução agendada (cron diário às 02:00)
* Filtro por branch (feature/*)
* Filtro por caminho com exceção (!src/docs/)
* Geração de relatórios
* Upload de artefatos
* Download de artefatos em outro job

## Validação

* Push na main → não executa
* Alteração em docs → não executa
* Alteração em código → executa
* Artefatos disponíveis para download

## Conclusão

O pipeline evita execuções desnecessárias e garante persistência dos arquivos gerados entre jobs.
