# Blue Team SOC Lab

Laboratório prático de cibersegurança defensiva (**Blue Team**) com foco no desenvolvimento de competências para atuação como **SOC Analyst Júnior**.

Este repositório documenta experimentos autorizados, procedimentos de análise, evidências sanitizadas, automações e lições aprendidas. O trabalho é incremental: cada etapa é validada antes de avançar.

## Objetivos

- Investigar configurações de segurança e a superfície de ataque em dispositivos próprios.
- Praticar coleta e interpretação de evidências técnicas usando ferramentas gratuitas.
- Desenvolver automações defensivas com Python.
- Evoluir gradualmente para um laboratório de monitoramento e resposta a incidentes.

## Ambiente de laboratório

- **Estação de análise:** Windows 11, PowerShell e Kali Linux no WSL2.
- **Dispositivo analisado:** smartphone Android de uso próprio, conectado por ADB (Android Debug Bridge) via Wi-Fi.
- **Abordagem:** consultas preferencialmente somente de leitura; alterações somente com decisão explícita do proprietário.
- **Custo:** priorização de ferramentas gratuitas e de código aberto.

> **Privacidade e ética:** endereços IP, números de série, nomes de dispositivos, credenciais, tokens, documentos pessoais e saídas brutas com dados sensíveis não devem ser publicados neste repositório.

## Progresso

| Área | Situação |
| --- | --- |
| Preparação da comunicação ADB via Wi-Fi | Realizada |
| Inventário inicial de pacotes Android | Realizado; análise individual em andamento |
| Identificação de origem de instalação de aplicativos | Em andamento |
| Revisão de serviços de acessibilidade ativos | Consulta realizada; nenhum serviço listado na evidência |
| Revisão de administradores de dispositivo | Consulta realizada; nenhum administrador ativo listado para o usuário principal |
| Auditoria de permissões especiais e sobreposição de tela | Próxima etapa |
| Coleta estruturada e sanitização de evidências | Planejada |
| Scripts de análise defensiva em Python | Planejados |
| Monitoramento de tráfego de rede | Planejado |
| SIEM, EDR e SOAR | Evolução futura, ainda não implementada |

**Importante:** ausência de indicadores em verificações específicas não comprova que um dispositivo esteja livre de ameaças. Da mesma forma, um nome de pacote desconhecido ou o instalador registrado não é evidência suficiente de malware.

## Metodologia

1. Definir o objetivo e o escopo de cada verificação.
2. Executar um procedimento por vez e registrar sua finalidade.
3. Interpretar resultados e distinguir fatos observados de hipóteses.
4. Documentar limitações e próximos passos.
5. Sanitizar evidências antes da publicação.

## Próximas etapas

- Revisar permissões especiais concedidas aos aplicativos, incluindo sobreposição de tela.
- Criar relatórios técnicos reproduzíveis sobre configurações e controles do Android.
- Elaborar scripts para inventário e comparação de pacotes.
- Avaliar, de acordo com a capacidade do ambiente, ferramentas de monitoramento e resposta como Wazuh (SIEM), Velociraptor (EDR/DFIR) e Shuffle (SOAR).

## Glossário

- **SOC** — Security Operations Center: centro de operações de segurança.
- **Blue Team** — equipe e atividades de defesa cibernética.
- **ADB** — Android Debug Bridge: interface de comunicação e diagnóstico Android.
- **SIEM** — Security Information and Event Management: centralização e correlação de eventos de segurança.
- **EDR** — Endpoint Detection and Response: detecção e resposta em endpoints.
- **SOAR** — Security Orchestration, Automation and Response: orquestração e automação de resposta.
- **DFIR** — Digital Forensics and Incident Response: forense digital e resposta a incidentes.

## Uso responsável

Os experimentos são realizados em ambientes e dispositivos próprios ou expressamente autorizados. Este projeto tem finalidade educacional e defensiva.

---

**Estado do projeto:** iniciado; documentação e análises em evolução.
