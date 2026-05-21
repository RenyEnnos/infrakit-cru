# Roteamento de Modos

Use este arquivo depois da entrevista inicial para decidir quais módulos carregar.

## Regra Geral

Não carregue tudo por padrão. Ative apenas os módulos que ajudam o trabalho atual.

## Modos Disponíveis

| Sinal no pedido | Arquivo a carregar | Motivo |
|---|---|---|
| proposta para direção, coordenação, universidade, órgão, cliente interno ou setor técnico | `modos/PROPOSTA_INSTITUCIONAL_TECNICA.md` | estrutura de decisão, riscos e pedido formal |
| PDF fornecido, versões parecidas, documento sem `.tex` original | `core/PDF_E_VERSOES.md` | escolher arquivo canônico e extrair texto |
| sistema, rede, intranet, dados pessoais, login, usuários, arquivos, logs, servidor | `core/LGPD_TI.md` | riscos de TI, segurança e privacidade |
| números fortes, custo, desempenho, garantia, conformidade, implantação | `core/VALIDACAO_E_ENTREGA.md` | separar fato, hipótese, validação e promessa |

## Saída Esperada

Depois de rotear, registre em `projeto/CONTEXTO_TRABALHO.md`:

- modo principal escolhido;
- módulos ativados;
- motivo da escolha;
- módulos não usados, se houver risco de confusão.

## Exemplo

Se o usuário trouxer uma proposta de intranet para uma universidade:

1. ativar `modos/PROPOSTA_INSTITUCIONAL_TECNICA.md`;
2. ativar `core/LGPD_TI.md`;
3. ativar `core/VALIDACAO_E_ENTREGA.md`;
4. ativar `core/PDF_E_VERSOES.md` se houver PDF.
