# Insights e Anotações: Infraestrutura Automatizada com CloudFormation

Aqui, registro minhas reflexões do desafio, baseadas nas aulas e prática. Como Code Girl, documentar me empodera a fixar conceitos e planejar carreira na AWS.

## Aprendizados Chave
- **Condições e Flexibilidade:** Usar Conditions evitou criar recursos desnecessários – ideal para pipelines CI/CD no Santander (ex.: bucket só em staging).
- **Tags Automáticas:** !Ref para Ambiente facilita governança (custos, segurança). Insight: Tags ajudam em queries no Cost Explorer.
- **Idempotência em Ação:** Re-deploy com mudança de parâmetro (ex.: CriarBucket "nao") rolou sem erros – CloudFormation é mágica!

## Desafios Enfrentados e Soluções
- **Erro em AllowedValues:** Parâmetro inválido causou falha na validação. Solução: Limitei opções (sim/nao) – teste sempre no Designer.
- **Monitoramento Avançado:** Eventos mostraram "UPDATE_IN_PROGRESS" em tags – aprendi a usar change sets para previews futuros.
- **Custos e Cleanup:** Zero charges, mas tags ajudam a trackear. Sempre delete stacks!

## Reflexões Pessoais
- Como mulher na tech, o bootcamp me mostrou que automação reduz bias em setups manuais. Futuro: Integrar com Lambda para serverless.
- Lição Geral: IaC é acessível – comece simples, evolua com condições. Isso me prepara para CLF-C02!

Obrigada, Santander! 💖