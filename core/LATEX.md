# Política de LaTeX

O Infrakit usa LaTeX como formato principal para documentos finais escritos.

## Por Que LaTeX

LaTeX facilita:

- controle de citações;
- sumário automático;
- formatação consistente;
- tabelas e figuras com numeração;
- geração de PDF reprodutível;
- adequação a normas acadêmicas.

## Verificação Inicial

Antes de escrever o documento final, o agente deve verificar se existe uma ferramenta LaTeX disponível.

Verificações comuns:

```bash
which pdflatex
which latexmk
which xelatex
which lualatex
```

Se nada estiver disponível, o agente deve pedir permissão antes de configurar.

## Regra de Permissão

O agente não deve instalar pacotes, baixar distribuições ou alterar configuração do sistema sem autorização do usuário.

Mensagem sugerida:

```text
Não encontrei LaTeX configurado. Para gerar o PDF final, preciso configurar uma ferramenta LaTeX. Posso fazer essa configuração?
```

## Preferência de Compilação

Ordem preferida:

1. `latexmk`, quando disponível;
2. `pdflatex` com passagens suficientes;
3. `xelatex` ou `lualatex`, se houver exigência de fonte específica.

## Estrutura Recomendada do Documento

Quando o trabalho já estiver pronto para produção, o agente pode criar uma estrutura como:

```text
trabalho/
  main.tex
  referencias.bib
  secoes/
  figuras/
  tabelas/
  build/
```

Essa estrutura só deve ser criada quando fizer sentido para o projeto. No início, o agente deve primeiro entender a entrega.

## Verificação Antes de Entregar

Antes de dizer que o PDF está pronto, o agente deve verificar:

- compilação sem erro fatal;
- sumário e referências atualizados;
- citações resolvidas;
- figuras aparecendo;
- tabelas dentro da página;
- PDF gerado no local correto;
- checklist de entrega coerente com o tipo de trabalho.
