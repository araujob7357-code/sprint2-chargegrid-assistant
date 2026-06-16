# sprint2-chargegrid-assistant
# ChargeGrid Assistant

## EV Challenge 2026 | GoodWe | FIAP

### Equipe 03

* Arthur Araujo Massarioli – RM 573308
* Beatriz da Silva Araújo – RM 570619
* Daniel Alejandro Pupo Martinez – RM 573075
* Victor Hugo Lavaqui – RM 573838
* Wendel Pedro Rezende – RM 573126

---

## Descrição do Projeto

O ChargeGrid Assistant é um chatbot inteligente desenvolvido para o EV Challenge 2026 da GoodWe.

O objetivo do sistema é auxiliar motoristas de veículos elétricos durante a utilização dos eletropostos da rede ChargeGrid Intelligence, fornecendo suporte em linguagem simples e acessível.

O chatbot é capaz de:

* Orientar o início da sessão de carregamento.
* Informar dados da sessão de recarga.
* Explicar a tarifação dinâmica.
* Explicar formas de pagamento (PIX, crédito e débito).
* Auxiliar no encerramento da sessão.
* Encaminhar problemas físicos para suporte técnico.

---

## Problema Resolvido

Muitos usuários de veículos elétricos encontram dificuldades durante o uso de eletropostos comerciais devido à falta de suporte imediato para dúvidas operacionais e problemas simples de utilização.

O ChargeGrid Assistant busca melhorar a experiência do usuário oferecendo atendimento conversacional diretamente pelo totem ou aplicativo móvel.

---

## Tecnologias Utilizadas

* Python
* Google Colab
* Google Gemini 2.5 Flash
* Inteligência Artificial Generativa

---

## Arquitetura da Solução

Fluxo de funcionamento:

1. Usuário envia uma mensagem.
2. O sistema injeta o contexto do ChargeGrid Assistant.
3. Dados da sessão são adicionados ao prompt.
4. O modelo Gemini gera a resposta.
5. A resposta é exibida ao usuário.
6. Problemas físicos podem ser direcionados ao suporte técnico.

---

## Funcionalidades Implementadas

### Início de Sessão

O chatbot orienta o usuário sobre como iniciar uma recarga de forma simples e objetiva.

### Informações da Sessão

Exibe informações como:

* Percentual da bateria
* Energia consumida
* Tempo restante
* Valor acumulado

### Tarifação Dinâmica

Explica a variação de preços conforme horário e demanda.

### Pagamentos

Suporte para:

* PIX
* Cartão de crédito
* Cartão de débito

### Encerramento da Sessão

Orienta o usuário sobre como finalizar a recarga e obter comprovantes.

### Escalamento para Suporte Técnico

Problemas físicos relacionados ao equipamento são encaminhados para atendimento presencial.

---

## Como Executar

### Instalar Dependências

```bash
pip install google-generativeai
```

### Configurar API Key

Criar uma API Key no Google AI Studio e configurar:

```python
import google.generativeai as genai

genai.configure(api_key="SUA_API_KEY")
```

### Executar o Chatbot

```python
conversar("Como eu começo a carregar meu carro aqui?")
```

---

## Exemplo de Uso

Pergunta:

Como eu começo a carregar meu carro aqui?

Resposta:

Para iniciar a recarga, conecte o cabo ao veículo, selecione a forma de pagamento desejada e confirme a operação. Após a confirmação, a sessão será iniciada automaticamente.

---

## Casos de Teste

Foram executados os testes definidos na Sprint 1:

* Início de sessão
* Progresso da recarga
* Tarifação dinâmica
* Problemas físicos
* Encerramento da sessão
* Pagamento via PIX

Os resultados demonstraram comportamento adequado dentro do contexto definido para o ChargeGrid Assistant.

---

## Repositório

(https://github.com/araujob7357-code/sprint2-chargegrid-assistant.git)
---

## Vídeo de Demonstração

(https://youtu.be/ZJoRZm1_1Hg)
