# Blue Team SOC Lab

Laboratório pessoal de **segurança defensiva**, com foco na construção de competências para **SOC Analyst L1**. O estágio atual é a auditoria autorizada de um smartphone Android próprio por meio de **ADB via Wi-Fi**, usando Windows 11, PowerShell e Kali Linux no WSL2.

> **Estado:** em desenvolvimento. Não é um SOC de produção. SIEM, EDR, SOAR e automações avançadas ainda são objetivos futuros, não implementações concluídas.

## Objetivos

- Investigar e documentar configurações de segurança de dispositivos próprios.
- Interpretar evidências sem atribuir automaticamente comportamentos a invasões ou malware.
- Desenvolver procedimentos reproduzíveis e, futuramente, automações defensivas com ferramentas gratuitas.
- Evoluir para coleta, análise e monitoramento de eventos em laboratório autorizado.

## Progresso

| Verificação | Situação |
| --- | --- |
| Comunicação ADB via Wi-Fi | Realizada |
| Inventário inicial de pacotes Android | Realizado; revisão em andamento |
| Origem de instalação de aplicativos | Investigação em andamento |
| Serviços de acessibilidade | Consulta realizada |
| Administradores de dispositivo | Consulta realizada |
| Permissões especiais e sobreposição de tela | Próxima etapa |
| Relatórios estruturados com evidências sanitizadas | Planejado |
| Scripts Python para inventário e comparação | Planejado |
| Monitoramento de tráfego | Planejado |
| SIEM, EDR e SOAR | Futuro; não implementado |

**Limitação:** uma consulta com resultado vazio não comprova a ausência de ameaças; um nome de pacote ou instalador desconhecido tampouco constitui, isoladamente, evidência de comprometimento.

## Procedimento de análise

1. Registrar objetivo, escopo e autorização.
2. Executar uma verificação por vez, compreendendo cada comando.
3. Conferir a saída e registrar apenas as observações comprovadas.
4. Separar fatos, hipóteses e limitações.
5. Revisar e sanitizar materiais antes de publicar relatórios.

## Proteção de dados

Nunca publicar evidências brutas contendo IPs pessoais, identificadores, nomes de dispositivos, contas, senhas, tokens ou outros dados sensíveis. O [`.gitignore`](.gitignore) ajuda a evitar inclusão acidental, mas não garante proteção de segredos: cada commit requer revisão manual.

## Evolução planejada

Concluir a auditoria de permissões Android, organizar relatórios técnicos, desenvolver rotinas defensivas em Python e iniciar estudos práticos com ferramentas de monitoramento e resposta quando o ambiente estiver preparado.

## Glossário

- **SOC:** Security Operations Center.
- **Blue Team:** defesa, detecção e resposta.
- **ADB:** Android Debug Bridge.
- **SIEM:** Security Information and Event Management.
- **EDR:** Endpoint Detection and Response.
- **SOAR:** Security Orchestration, Automation and Response.
- **DFIR:** Digital Forensics and Incident Response.

Todos os experimentos são realizados em equipamentos próprios ou com autorização expressa.
