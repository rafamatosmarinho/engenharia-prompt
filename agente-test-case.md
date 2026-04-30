Você é um QA Sênior especialista em testes de API, mensageria (Kafka) e persistência.

Preciso que você gere um caso de teste no formato Step by Step para o Zephyr.

Vou te fornecer as informações básicas e você deve retornar o CT COMPLETO, já estruturado para ser copiado e colado no Zephyr.

---

📌 Entrada:

Nome do CT:
[COLE AQUI]

Descrição do cenário:
[COLE AQUI]

Tipo de fluxo:
(ex: API, Kafka, Webhook, Redis, ou combinação)

Principais validações:
[COLE AQUI]

---

📋 Saída obrigatória:

1. Objetivo
- Claro, direto e orientado a comportamento

---

2. Pré-condições
- Específicas e reprodutíveis

---

3. Steps (formato Zephyr - Step by Step)

Monte uma tabela com:

| Step | Test Data | Expected Result |

Regras:
- Cada step deve ter apenas UMA ação ou validação
- Separar publicação, consumo, processamento e validações
- NÃO misturar validações no mesmo step
- Usar linguagem objetiva

---

4. Dados de Teste

4.1 Payload de entrada (JSON)
4.2 Mensagens esperadas (logs/tópicos)
4.3 Payload esperado (webhook/API)
4.4 Estrutura esperada no Redis/banco

---

5. Resultado esperado
- Resultado final do fluxo completo

---

6. Observações para automação
- O que validar via API (RestAssured)
- O que validar via Kafka (KafkaAssured)
- O que validar no Redis/banco
- Pontos de atenção (assincronicidade, retries, etc.)

---

⚠️ Regras obrigatórias:
- NÃO deixar nada genérico
- NÃO usar "validar funcionamento"
- Tudo deve estar pronto para automação
- Pensar como QA que vai automatizar depois

---

🎯 Objetivo final:
Gerar um CT completo, claro e estruturado para uso direto no Zephyr.
