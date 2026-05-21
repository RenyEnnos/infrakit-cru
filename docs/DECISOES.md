# Decisões do Framework

Registro curto de decisões arquiteturais do Infrakit Cru.

## 2026-05-21 - Separar núcleo fixo de arquivos vivos

O Infrakit foi dividido em `core/`, `agente/`, `projeto/` e `docs/`.

Motivo: permitir que o agente adapte o trabalho sem modificar as regras permanentes do framework.

## 2026-05-21 - Manter LaTeX como regra fixa

O documento final escrito deve ser produzido em LaTeX, salvo exigência formal diferente.

Motivo: preservar compilação reprodutível, controle de referências e formatação acadêmica.

## 2026-05-21 - Usar logs híbridos

O registro principal fica em `projeto/REGISTRO_ITERACOES.md`, e detalhes longos vão para `projeto/logs/`.

Motivo: manter histórico navegável sem perder evidência de iterações grandes.

## 2026-05-21 - Não assumir TCC como padrão

O agente deve entrevistar o usuário antes de adaptar a rubrica e checklist.

Motivo: o mesmo framework deve servir para TCC, artigo, relatório, seminário, revisão bibliográfica e outros tipos de entrega.
