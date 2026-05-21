# PDF e Controle de Versões

Use este protocolo quando o usuário fornecer PDF, houver mais de uma versão parecida ou for necessário reconstruir um documento a partir de PDF.

## Objetivo

Evitar trabalhar no arquivo errado e deixar registrado qual versão foi usada como fonte.

## Protocolo de Arquivo Canônico

1. Localize os arquivos candidatos.
2. Liste nome, caminho, tamanho e data de modificação.
3. Gere hash do arquivo escolhido.
4. Extraia metadados básicos.
5. Extraia texto para leitura.
6. Confirme com o usuário quando houver ambiguidade relevante.
7. Registre o arquivo canônico em `projeto/CONTEXTO_TRABALHO.md`.

Comandos úteis:

```bash
sha256sum arquivo.pdf
pdfinfo arquivo.pdf
pdftotext -layout arquivo.pdf saida.txt
```

Se `pdfinfo` ou `pdftotext` não estiverem disponíveis, registre a limitação e use a melhor alternativa disponível.

## Quando Há PDFs Parecidos

Compare:

- título;
- número de páginas;
- data de modificação;
- hash;
- primeiras linhas extraídas;
- nomes de autores;
- presença de anexos ou tabelas;
- versão declarada no próprio documento.

Não avalie a qualidade final antes de ter alta confiança de que o PDF correto foi escolhido.

## Registro Recomendado

Use uma tabela como esta:

| Arquivo | SHA256 | Páginas | Status | Observação |
|---|---|---:|---|---|
| preencher | preencher | preencher | candidato/canônico/descartado | preencher |

## Reconstrução em LaTeX

Se o usuário só tiver PDF e precisar de um `.tex` editável:

1. extraia o texto;
2. identifique estrutura provável;
3. reconstrua em LaTeX com seções limpas;
4. recrie tabelas manualmente quando necessário;
5. não preserve erros de layout do PDF original;
6. compile;
7. compare visualmente o PDF novo com o original quando a fidelidade for importante.

## Problemas de Layout em PDF

Verifique especialmente:

- tabelas quebradas;
- texto fora da margem;
- imagens de baixa resolução;
- numeração incoerente;
- referências cortadas;
- páginas em branco inesperadas;
- seções iniciando no lugar errado.

Registre problemas encontrados em `projeto/CHECKLIST_ENTREGA.md` ou no log da iteração.
