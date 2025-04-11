# Visão Geral do Projeto

## Objetivo

Este projeto tem como objetivo principal proporcionar uma experiência prática com diferentes paradigmas de comunicação em sistemas distribuídos. Você irá implementar um subsistema de checkout de um comércio eletrônico utilizando duas abordagens distintas:

1.  **Comunicação Síncrona baseada em RPC:** Utilizando gRPC ou Web Services REST.
2.  **Comunicação Assíncrona baseada em Publish-Subscribe:** Utilizando Apache Kafka.

Ao final, deverá ser feita uma comparação das duas arquiteturas, analisando suas características, vantagens, desvantagens e, principalmente, seu comportamento em relação à escalabilidade e ao tratamento de altas cargas de trabalho.

## Contexto: O Fluxo de Checkout

Imagine um sistema de comércio eletrônico. Quando um cliente finaliza a compra (checkout), diversas etapas precisam ser executadas em sequência ou em paralelo:

1.  **Criação do Pedido:** O pedido inicial é registrado no sistema.
2.  **Processamento do Pagamento:** O pagamento é verificado e autorizado.
3.  **Separação de Estoque:** Os itens do pedido são localizados e separados no estoque.
4.  **Emissão da Nota Fiscal:** Uma nota fiscal é gerada para o pedido.
5.  **Envio para Transportadora:** O pedido é despachado para a empresa de logística/transportadora.

Este fluxo envolve múltiplos "serviços" ou responsabilidades que precisam se comunicar.

O restante da especificação está no documento PDF.
