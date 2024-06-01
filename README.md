# Projeto recusa / liberação de vendas
Este projeto, focado no módulo SD(Sales and Distributions), busca praticar a construção de relatórios ALV utilizando a classe CL_GUI_ALV_GRID, module pool e BAPI. Com base em um range de números de documentos de vendas passado na tela de seleção,
ocorre a seleção dos itens de venda na tabela VBAP e a exibição dos mesmos. Caso o usuário queira bloquear a venda de um determinado item, ele deve selecionar uma linha no ALV e clicar no botão "Recusar", definindo o campo ABGRU da tabela transparente VBAP para '00'. Por outro lado, se o usuário deseja liberar a venda do item, ele precisa selecionar uma linha no ALV e clicar no botão "Liberar", definindo o campo ABGRU da tabela transparente VBAP para vazio.
Tal processo ocorre mediante o uso da BAPI (módulo de função que permite realizar uma função empresarial específica) denominada 'BAPI_SALESORDER_CHANGE'.

## Tela de seleção

