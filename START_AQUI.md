# Start Aqui

Este é o arquivo de entrada do Infrakit Cru.

Se você é o usuário, diga ao agente:

```text
Leia este arquivo e siga o protocolo do Infrakit.
```

Se você é o agente, execute a sequência abaixo sem pular etapas.

Todos os caminhos citados neste kit são relativos à raiz da pasta `infrakit_cru/`.

## Sequência Obrigatória do Agente

1. Ler `agente/PROMPT_AGENTE.md`.
2. Ler `core/REGRAS_FIXAS.md`.
3. Ler `core/LATEX.md`.
4. Ler `agente/ENTREVISTA_INICIAL.md`.
5. Verificar se os arquivos vivos em `projeto/` já foram preenchidos.
6. Se o contexto ainda estiver incompleto, entrevistar o usuário em linguagem simples.
7. Atualizar os arquivos em `projeto/` com base nas respostas.
8. Confirmar ao usuário o que foi entendido.
9. Só então iniciar redação, revisão, pesquisa, avaliação ou formatação.

## O Que o Agente Pode Modificar

O agente pode modificar os arquivos em `projeto/`:

- `CONTEXTO_TRABALHO.md`
- `RUBRICA.md`
- `CHECKLIST_ENTREGA.md`
- `SCORECARD.md`
- `BASE_CONHECIMENTO.md`
- `REFERENCIAS_CANDIDATAS.md`
- `REGISTRO_ITERACOES.md`
- arquivos dentro de `logs/`, quando uma iteração precisar de registro detalhado

O agente não deve modificar `core/` durante um trabalho comum. A pasta `core/` é a base fixa do framework.

## Primeira Resposta Esperada do Agente

O agente deve começar explicando, em poucas linhas:

1. que vai fazer uma entrevista curta;
2. que o usuário pode responder com "não sei";
3. que o objetivo é adaptar o Infrakit ao tipo real de trabalho;
4. que nenhuma escrita final começa antes do contexto mínimo estar claro.
