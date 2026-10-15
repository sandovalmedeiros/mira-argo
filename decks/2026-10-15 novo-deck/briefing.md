# Briefing: Projeto ARGO (pitch para stakeholders)

**Fonte:** Projeto_ARGO_Relatorio_Concepcao_Proposta_v0.6_Stakeholders.pdf (pdf) + Arquitetura ARGO_ Governança Orientada por IA.png + _tema.md
**Path:** decks/2026-10-15 novo-deck/references/
**Data da extração:** 2026-10-15

## Essência em uma frase

O Projeto ARGO propõe um framework institucional de Harness Engineering para a SEI/DIGEO/CGEO estruturar o uso de IA no desenvolvimento, modernização e governança de software, substituindo a visão de "IA como assistente de programação" por um modelo coordenado de agentes, regras e evidências, e pede à gestão a autorização de uma Prova de Conceito controlada, sem compromisso prévio de adoção de tecnologia ou fornecedor.

## Conceitos-chave (candidatos a slide)

1. **Do assistente ao Harness Engineering**: IA como assistente vs. modelo institucional onde agentes, modelos, ferramentas, padrões, segurança, testes, observabilidade e aprovação humana operam coordenados. É a virada de mentalidade do pitch. Sugestão: `comparacao`
2. **A tese**: o valor institucional reside em princípios, padrões, ADRs, políticas, contratos, autonomia, evidências, conformidade e observabilidade; modelos e orquestradores são componentes substituíveis. Sugestão: `comparacao`
3. **O problema**: modelos isolados não conhecem regras institucionais, arquitetura, legado, segurança, integrações; uso corporativo exige contexto, ferramentas autorizadas, identidade, auditoria, limites de custo e aprovação. Sugestão: `d3-fluxo`
4. **O Harness (camada operacional)**: entre decisões institucionais e agentes ficam Context Engineering, Guardrails, Skills, MCP/Tools, identidade/RBAC, Policy as Code, Quality Gates, testes, observabilidade, Evidence by Design, FinOps e human-in-the-loop. Sugestão: `d3-fluxo` (camadas empilhadas)
5. **Modelo operacional em 4 planos**: Governance, Control, Execution e Observability; a inteligência institucional mora nos planos de Governance e Control, reduzindo dependência de tecnologia específica. A Figura 2 do relatório e o PNG de arquitetura referem-se a isso. Sugestão: `d3-fluxo` ou `comparacao`
6. **Autonomia A0-A5**: escada de consultivo (A0) a ação privilegiada com auditoria reforçada (A5); autonomia concedida por risco e contexto, nunca só pela capacidade do modelo. Sugestão: `timeline` (escada) ou `metricas`
7. **Classificação de regras**: PROIBIDO, INEGOCIÁVEL, PREFERENCIAL, CONTEXTUAL; microserviços, Kubernetes, RAG etc. não são dogmas, princípios fortes podem ser obrigatórios e tecnologias são meios contextuais. Sugestão: `comparacao` (matriz 2x2)
8. **Reversa como encurtador de caminho**: produz evidência do AS-IS, não norma; ciclo maduro de minerar, comparar, priorizar, modernizar, validar e reminerar (Architecture Fitness). Sugestão: `timeline` (ciclo)
9. **Estratégia de orquestração**: definir primeiro o Orchestration Contract; Hermes é baseline, não dependência arquitetural; comparação com o mesmo caso de uso; decisão em ADR. Sugestão: `d3-fluxo`
10. **Decision Gate Build vs. Adopt**: desenvolvimento próprio só quando evidências e Business Case justificarem (o custo oculto de um orquestrador próprio: estado, memória, filas, retries, segurança, suporte). Sugestão: `d3-fluxo` (porte/funil)
11. **Ecossistema a avaliar**: Hermes, LangGraph/Deep Agents, Microsoft Agent Framework, CrewAI, OpenAI Agents SDK, Claude Agent SDK, Google ADK, LlamaIndex Workflows (8 alternativas, papéis distintos). Sugestão: `comparacao` (tabela)
12. **Segurança**: ameaças consideradas incluem prompt injection, tool poisoning, exfiltração, secrets, escalada de privilégios, execução destrutiva, supply chain, loops, adulteração de evidências e MCPs privilegiados; a Baseline v0.6.1 adiciona Conformance Suite, Budget Envelope e Model Routing. Sugestão: `metricas` ou `comparacao`
13. **Riscos e mitigações**: 9 pares (institucionalizar erros do legado, rigidez excessiva, overengineering, lock-in, infraestrutura prematura, autonomia excessiva, documentação sem execução, custo imprevisível, evidência insuficiente). Sugestão: `comparacao` (tabela)
14. **Implantação em 6 passos**: Aprovação, Baseline Técnica, Piloto (sistema CGEO de risco controlável), PoC (ciclo completo), Avaliação (segurança, conformidade, custos, produtividade), Deliberação (continuidade, ajustes, adoção, extensão ou subprojeto). Sugestão: `timeline`
15. **Critérios de sucesso da PoC**: 100% dos requisitos críticos P0, rastreabilidade ponta a ponta, zero exposição de secrets, nenhuma ação fora da policy, evidências auditáveis, custo mensurável, substituibilidade prevista, dados para Build/Adopt/Extend. Sugestão: `metricas`
16. **O que o ARGO NÃO é**: não é Hermes, Claude, Reversa, BMAD, novo modelo de IA nem obrigatoriamente novo produto de software; desarma objeções antes do pedido. Sugestão: `comparacao`
17. **A deliberação (CTA)**: aprovar o ARGO como iniciativa experimental e autorizar a PoC controlada conforme Baseline v0.6.1, sem compromisso prévio de contratação, aquisição, implantação produtiva ou plataforma própria. Sugestão: slide de fecho com o pedido formal
18. **Frase-manifesto** (abre e fecha o documento): "A IA não governa a arquitetura; a arquitetura governa a IA." Sugestão: capa e/ou fecho

## Dados e números

- Documento: versão 0.6, de 06/10/2026; Baseline Técnica companion: v0.6.1
- 4 planos operacionais (Governance, Control, Execution, Observability)
- 6 níveis de autonomia (A0 a A5)
- 4 classes de regra (PROIBIDO, INEGOCIÁVEL, PREFERENCIAL, CONTEXTUAL)
- 8 alternativas de ecossistema a avaliar
- 9 riscos com mitigações mapeadas
- 6 etapas de implantação
- Critério de sucesso objetivo: 100% dos requisitos críticos P0, zero exposição de secrets, zero ações fora da policy
- Papéis fixados: Reversa (Architecture Mining/AS-IS), BMAD (análise/TO-BE), Hermes (baseline de orquestração), Claude Code/CLI (opção de execução), Governança Arquitetural (autoridade)

## Trechos de código emblemáticos

Não há: o documento é conceitual/gerencial, sem código. As Figuras 1 a 4 (Fluxo Integrado, Quatro Planos, Policy as Code, Decision Gate) são descritas em texto e são candidatos fortes a animações D3 originais em vez de prints.

## Narrativa sugerida

Problema (modelos isolados não conhecem a instituição; adoção fragmentada) → virada de mentalidade (Harness Engineering institucional) → tese (valor em princípios e evidências, tecnologia é substituível) → como funciona (4 planos, Harness, A0-A5, Policy as Code, Evidence by Design) → o que não é (desarma objeções) → riscos e mitigações (credibilidade) → caminho de implantação em 6 passos → critérios de sucesso objetivos → CTA: autorizar a PoC controlada, fechando com o manifesto "A IA não governa a arquitetura; a arquitetura governa a IA."

## Lacunas

- Benefícios são qualitativos: não há ROI, prazos nem custos estimados no documento (se houver números de negócio, vale incluir na versão final do pitch)
- Nomes/cargo do apresentador e data da reunião de deliberação não constam
- Duração alvo do pitch (número de minutos ou slides) não definida
- Decidir se o PNG "Arquitetura ARGO" entra como imagem posicionada (via /mira-image) ou se as figuras são recriadas como animações D3 (recomendado pelo padrão Mira)
- Identidade institucional (brasão SEI/DIGEO/CGEO), se precisar aparecer na capa
