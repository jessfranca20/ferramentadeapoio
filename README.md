# Ferramenta de Apoio — Pós-Venda

Ferramenta web para apoio às atividades do dia a dia do pós-venda. Roda inteiramente no navegador, sem instalação e sem servidor — basta abrir o arquivo.

## Funcionalidades

A ferramenta tem quatro abas:

1. **📅 Prazo de Entrega** — calcula o prazo de entrega em dias úteis (10, 20 ou 30 dias + 5 de tolerância) a partir da data da compra e gera a mensagem pronta para enviar ao cliente.

2. **⚖️ Cálculo de Multa** — calcula a multa e os juros por atraso ou cancelamento conforme a Cláusula Quarta do contrato (1% fixo + 0,5% ao mês por mês cheio, contados após o prazo máximo com tolerância).

3. **🛡️ Contestação** — gera a defesa formal de contestação de cartão (chargeback) para envio à operadora, com quatro cenários pré-configurados.

4. **🧾 Recibo** — gera recibo de pagamento com valor por extenso e exportação em PDF.

## Como usar

Basta abrir o arquivo `index.html` em qualquer navegador (Chrome, Edge, Firefox, Safari). Funciona em computador e celular.

## Observações

- Os feriados considerados nos cálculos de prazo são os nacionais brasileiros de 2025 e 2026. Feriados municipais e estaduais não estão incluídos — confira sempre o calendário local.
- Todos os cálculos rodam localmente no navegador. Nenhum dado é enviado para fora.
- O recibo gerado é um comprovante de pagamento e não substitui a nota fiscal.

## Tecnologia

Arquivo HTML único, com JavaScript puro. A geração de PDF usa a biblioteca [jsPDF](https://github.com/parallax/jsPDF), carregada via CDN.
