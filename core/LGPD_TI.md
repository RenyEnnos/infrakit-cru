# LGPD e TI Institucional

Use este módulo quando o trabalho envolver sistemas, redes, usuários, contas, dados pessoais, logs, autenticação, arquivos, comunicação interna, internet, infraestrutura ou implantação tecnológica.

Este módulo não substitui parecer jurídico ou técnico. Ele ajuda a não ignorar riscos básicos.

## Perguntas de Acionamento

Se qualquer resposta for "sim", aplique o checklist:

1. O projeto envolve cadastro de usuários?
2. Haverá login, senha, e-mail, matrícula, nome ou cargo?
3. O sistema armazena mensagens, arquivos, logs ou histórico?
4. A solução roda em rede institucional?
5. A proposta depende de servidor, roteador, firewall, Docker, domínio ou porta exposta?
6. Há uso por alunos, servidores, professores ou público externo?
7. A implantação depende da TI, direção ou setor administrativo?

## Checklist LGPD

- [ ] Dados pessoais identificados
- [ ] Finalidade de uso declarada
- [ ] Base legal ou justificativa institucional marcada como pendência
- [ ] Minimização de dados considerada
- [ ] Controle de acesso previsto
- [ ] Retenção de dados tratada
- [ ] Exclusão ou encerramento de contas tratado
- [ ] Termo de uso ou aviso de privacidade marcado como necessário, se aplicável
- [ ] Responsável institucional identificado ou marcado como pendência
- [ ] Riscos de exposição de dados mencionados sem promessa absoluta

## Checklist Técnico

- [ ] Responsável técnico identificado ou pendente
- [ ] Ambiente de hospedagem descrito
- [ ] Backup considerado
- [ ] Atualizações e manutenção consideradas
- [ ] Logs tratados com finalidade e retenção
- [ ] Autenticação considerada
- [ ] Isolamento de rede considerado
- [ ] Acesso externo tratado, se houver
- [ ] Plano de resposta a incidente mencionado ou marcado como pendência
- [ ] Validação da TI indicada como requisito antes de produção

## Linguagem Segura

Evite:

- "totalmente seguro";
- "sem risco";
- "em conformidade com a LGPD" sem validação;
- "não coleta dados" sem mapear logs, usuários e arquivos;
- "não exige manutenção".

Prefira:

- "a proposta prevê medidas de segurança";
- "a conformidade depende de validação institucional";
- "os dados pessoais devem ser minimizados";
- "a implantação em produção requer revisão da TI";
- "o piloto deve ocorrer em ambiente controlado".

## Registro de Pendências

Quando algo não estiver validado, registre explicitamente:

| Pendência | Responsável provável | Impacto |
|---|---|---|
| validação da TI | setor de TI / direção | requisito antes de produção |
