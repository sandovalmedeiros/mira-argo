# Roteiro de narração: Projeto ARGO (pitch de deliberação)

**Como usar:** cada bloco abaixo é o que você fala quando o slide correspondente está na tela. Frases curtas, linguagem simples, prontas para ler ou decorar. Tempo estimado: 10 a 12 minutos no total (30 a 45 segundos por slide). Navegue com a seta do teclado; F alterna tela cheia.

---

## Slide 1 · Capa

Bom dia a todos. O que vocês vão ver agora é o Projeto ARGO, a nossa proposta para usar inteligência artificial no desenvolvimento de software de forma segura e controlada. A frase no fundo resume tudo: a IA não governa a arquitetura; a arquitetura governa a IA. Ou seja: a tecnologia trabalha, mas quem manda são as nossas regras. No final, vou fazer um pedido simples: autorizar um teste controlado. Vamos lá.

## Slide 2 · 6 lacunas entre a IA e o corporativo

Começando pelo problema. Uma IA sozinha não conhece a nossa instituição. Ela não sabe quais são as nossas regras, não conhece os nossos sistemas antigos, não tem permissões, não deixa registro do que fez, não controla custo e não pede autorização para ninguém. São esses seis buracos que aparecem na tela. Enquanto eles existirem, usar IA no corporativo é correr risco sem necessidade.

## Slide 3 · Do copiloto ao harness

A mudança que o ARGO propõe é de mentalidade. Hoje tratamos a IA como um assistente: cada um usa do seu jeito, sem memória e sem controle. A proposta é tratar a IA como um profissional dentro de um ambiente preparado: com contexto, ferramentas autorizadas, padrões, testes e registro de tudo o que faz. Esse ambiente preparado é o que chamamos de harness.

## Slide 4 · 12 barreiras entre o modelo e o risco

Neste desenho, a IA está no centro, e ao redor dela estão as doze proteções do ARGO: contexto, regras de segurança, ferramentas controladas, verificação de qualidade, teste, monitoramento, registro de evidências, controle de custo e aprovação humana, entre outras. A mensagem é simples: nenhuma ação da IA acontece por fora dessas barreiras. E reparem no detalhe: o centro é substituível. Se amanhã surgir um modelo melhor, trocamos o centro sem mexer nas proteções.

## Slide 5 · 4 planos, 1 linha de autoridade

O ARGO se organiza em quatro planos, que vocês vêem se revezando na frente da tela. No plano de governança ficam os princípios e as decisões arquiteturais. No plano de controle ficam as regras aplicadas na prática, os portes de qualidade e a régua de autonomia. No plano de execução trabalham os agentes, com as ferramentas. E no plano de observabilidade fica o registro de tudo: evidência, rastro e custo. O importante: quem manda está em cima, e quem executa está embaixo. Se quiser ler um plano com calma, é só parar o mouse sobre o desenho que o rodízio pausa.

## Slide 6 · A arquitetura em uma tela

Esta é a figura oficial do relatório de concepção. Ela mostra a mesma ideia do slide anterior no formato de diagrama: os quatro blocos e o caminho que a regra percorre até virar evidência. Deixei aqui porque é a versão que está no documento que vocês receberam, para todos acompanharem no mesmo desenho.

## Slide 7 · 6 níveis de autonomia, zero atalhos

Aqui está a régua de liberdade da IA, do A0 ao A5. No A0, a IA só opina; nada é alterado. No A1, ela produz trabalhos, mas quem decide e executa é pessoa. Vai subindo até o A5, em que a IA pode executar ações sensíveis, mas com autorização explícita e auditoria reforçada. A regra de ouro está no rodapé: autonomia se concede pelo risco da tarefa, nunca pela capacidade do modelo. Se ele é bom, não significa que pode tudo.

## Slide 8 · O que pedimos hoje

Chego ao pedido central, adiantado de propósito. Pedimos a autorização para rodar uma Prova de Conceito, um teste controlado, seguindo a especificação técnica que já preparamos. Sem compromisso de compra, sem vinculação com fornecedor e sem decisão de construir nada próprio. O teste existe para produzir provas. Com provas na mão, a decisão de ir adiante fica muito mais fácil.

## Slide 9 · Proibido, inegociável, preferencial, contextual

Para não virar rigidez demais, as regras do ARGO têm quatro tipos. Tem coisa que é proibida, ponto. Tem princípio que é inegociável, como aprovação humana em ação crítica. Tem padrão recomendado, que admite exceção justificada. E tem a regra contextual, que depende do problema. É aí que entram microserviços, Kubernetes, RAG e companhia: são meios, e cada caso decide se precisa. Nenhuma tecnologia vira dogma.

## Slide 10 · O legado vira evidência, não palpite

O ARGO aproveita o que já temos. Com a ferramenta de mineração, o sistema legado é lido e transformado em evidência do que existe hoje. Depois comparamos com o que deveria ser, priorizamos, modernizamos, validamos e recomeçamos o ciclo. É um círculo que nunca termina, e é isso que mantém a arquitetura viva. E atenção: o resultado é prova do que existe, não norma do que deve existir.

## Slide 11 · Adotar primeiro, construir só com prova

Sobre a ferramenta de orquestração, a estratégia é começar adotando o que existe, com o Hermes como referência inicial, e comparar alternativas com o mesmo caso de uso. Construir um orquestrador próprio é assumir um produto inteiro: estado, memória, filas, segurança, atualização, suporte. Só vale quando as evidências e o business case justificarem. Por isso existe um porte de decisão: construir só com prova.

## Slide 12 · 8 alternativas, 1 critério: substituibilidade

Aqui está o ecossistema que vamos avaliar na comparação: oito opções, cada uma com um papel no estudo. O critério que atravessa todas é um só: poder trocar. Se uma tecnologia nos prende demais, ela entra em desvantagem na avaliação, e a decisão fica registrada em documento arquitetural, com o motivo.

## Slide 13 · 9 ameaças, 3 travas de fábrica

Sobre segurança, preferimos começar assumindo que tudo pode dar errado. Estão mapeadas nove ameaças, de injeção de prompt a ferramenta envenenada. E a especificação técnica já nasce com três travas de fábrica. A suíte de conformidade verifica automaticamente se tudo o que a IA entrega segue as regras: não passou no teste, não sai. O envelope de orçamento é o teto de custo: cada execução tem um limite de gasto, e se estourar, a ação para. E o roteamento de modelos escolhe o modelo certo para cada tarefa, pelo custo e pela capacidade, sem depender de um único fornecedor. Ou seja: segurança não é promessa futura, já vem no desenho.

## Slide 14 · 9 riscos, 9 mitigações, 0 surpresas

Este é o mapa de riscos do projeto. Cada risco da coluna da esquerda tem uma resposta na direita. Se o medo é consolidar os erros do passado, a resposta é evidência, não norma. Se o medo é autonomia demais, a resposta é a régua A0 a A5. Se é custo imprevisível, é FinOps com teto de orçamento. Risco mapeado com resposta deixa de ser surpresa.

## Slide 15 · Da aprovação à deliberação em 6 passos

O caminho é este: aprovar a iniciativa, padronizar com a baseline, escolher um piloto de risco controlado na CGEO, executar a PoC com regras e registros, avaliar segurança, conformidade, custo e produtividade, e só então deliberar: continuar, ajustar, adotar, ampliar ou transformar em subprojeto. Seis passos claros, do sim de hoje até a decisão de amanhã.

## Slide 16 · O ARGO em uma tela

Esta é a visão de síntese do projeto em uma única imagem, com a marca ARGO ao centro. Ao redor dela, os quatro pilares: governança orientada por IA, autonomia progressiva, evidência por desenho e substituibilidade. Se alguém perguntar o que é o ARGO em trinta segundos, é este desenho.

## Slide 17 · Os resultados esperados

E o que a instituição ganha com tudo isso? São seis resultados, exatamente os do infográfico oficial, com os ícones originais na tela. Código com mais qualidade e menos defeito. Velocidade que escala sem perder o controle. Governança que funciona de verdade, com rastro e auditoria. O conhecimento da casa no centro da geração de software, em vez de na cabeça de poucos. Uso responsável de IA, com autonomia na medida certa e gente no circuito. E valor público: mais eficiência e transparência com menos risco. E atenção à nota de rodapé: nada disso é promessa, é o que a PoC vai validar.

## Slide 18 · Sucesso tem número: 100% dos P0

E como vamos saber se o teste deu certo? Com números, não com impressão. Cem por cento dos requisitos críticos entregues. Zero senha exposta. Zero ação fora da regra. Rastro de ponta a ponta, custo medido e dados suficientes para decidir construir, adotar ou ampliar. É essa objetividade que protege a decisão de vocês.

## Slide 19 · A decisão de hoje: autorizar o experimento

Fechando com o pedido formal: aprovar o Projeto ARGO como iniciativa experimental e autorizar a Prova de Conceito controlada, conforme a baseline técnica, sem compromisso prévio com tecnologia, fornecedor ou desenvolvimento próprio. As evidências vão responder as próximas perguntas. E o critério de sucesso já está definido. A IA não governa a arquitetura; a arquitetura governa a IA. Obrigado.

---

## Glossário para o apresentador (os termos técnicos em linguagem simples)

Use estas definições na hora das perguntas, ou para enriquecer a fala se o público pedir detalhes.

- **Overengineering**: construir mais do que o problema pede. É a solução sofisticada para uma necessidade simples: encarece o projeto, complica a manutenção e não traz benefício real nenhum. No ARGO, o antídoto é não impor tecnologia sem necessidade.
- **FinOps**: a gestão financeira do uso de tecnologia: medir, acompanhar e controlar quanto cada execução custa, para o gasto ser previsível e justificado. FinOps vem de "financial operations", operações financeiras do consumo de nuvem e IA.
- **Budget Envelope**: o teto de gasto. Cada tarefa ou execução recebe um "envelope" com limite de custo; quando atinge o limite, a ação para em vez de continuar gastando. É travilha de fábrica na Baseline v0.6.1.
- **Model Routing**: o direcionador de modelos. Para cada tarefa, ele escolhe qual modelo de IA usar: o mais barato que resolve, ou o mais capaz quando a tarefa exige. Permite trocar e comparar fornecedores sem dependência de um só.
- **Lock-in**: a prisão tecnológica. Ficar tão dependente de um fornecedor ou de uma tecnologia que trocar vira caro ou inviável. O antídoto do ARGO: contratos e componentes substituíveis.
- **Decision Gate Build vs. Adopt**: o porte de decisão "construir ou adotar". Uma barreira formal que obriga a comparar adotar uma solução existente versus construir a própria, e só autoriza a construção quando as evidências e o business case justificarem.
- **Policy as Code**: a regra virando código. Em vez de política escrita em documento (que ninguém consegue obrigar), a regra é implementada como código que o sistema executa e verifica sozinho. Descumprir fica tecnicamente difícil, não depende de boa vontade.
- **Quality Gates**: os portes de qualidade. Pontos de checagem obrigatórios no fluxo de trabalho: o avanço só acontece se passar nos critérios de teste, segurança e revisão. Não passou, fica retido até passar.
- **Evidence by Design**: evidência por desenho. A prova não é montada depois, quando alguém pergunta: ela nasce embutida na ação. Toda ação relevante registra, por padrão, quem executou, qual política aplicou, qual modelo e ferramenta usou, qual foi o resultado e quem aprovou. É a mitigação do risco "evidência insuficiente" (slide 14).
- **Rastreabilidade**: o rastro de ponta a ponta. A capacidade de reconstruir depois, passo a passo, a história de qualquer decisão ou alteração: quem fez, o quê, quando, com qual ferramenta e sob qual aprovação. Sem rastro, não há auditoria possível; com rastro, a confiança vira fato verificável.
- **ADR**: o registro de decisão arquitetural (do inglês "Architecture Decision Record"). Um documento curto e numerado que registra uma decisão importante: o contexto, as opções consideradas, a escolha feita e o motivo. Meses depois, qualquer pessoa entende por que a arquitetura é assim, sem depender da memória de quem decidiu. No ARGO, decisões como construir ou adotar um orquestrador ficam registradas em ADR (slides 5, 11 e 12).

---

**Dicas de apresentação**

- Leve em média 40 segundos por slide; os slides 8 e 19 são os mais importantes, não tenha pressa neles.
- No slide 5, pare o mouse sobre o desenho para pausar o rodízio e deixar um plano fixo enquanto fala dele.
- Se o público for misto (técnico e gestor), os slides 4, 10 e 12 podem ser acelerados; 8, 15 e 18 merecem peso.
- Termine sempre apontando para a frase final: ela é o resumo memorável do projeto.
