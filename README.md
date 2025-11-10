# FF---C
desenvolvendo FF em C

Este commit estabelece as funcionalidades essenciais para a gestão de itens.

Funcionalidade Principal
Mochila Virtual: Implementação de uma lista sequencial estática (vetor) com capacidade máxima de 10 para armazenar itens.

Gestão de Itens: O sistema permite ao jogador cadastrar, remover, listar e buscar itens.

Conceitos e Estruturas Implementados
struct Item: Definição da estrutura para agrupar as informações de cada item: nome, tipo (arma, munição, cura) e quantidade.

Vetor Estático: Utilizado um vetor (mochila[10]) para representar a lista sequencial de itens.

Modularização: O código está organizado em funções claras, seguindo o padrão da lista sequencial:

inserirItem()

removerItem(): Implementa a lógica de deslocamento para preencher o espaço vazio após a remoção.

listarItens()

buscarItem(): Utiliza busca sequencial para localizar o item pelo nome.

Usabilidade: Implementação de um menu interativo (main) que permite ao usuário controlar o fluxo do inventário.
