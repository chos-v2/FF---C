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

Este commit marca uma expansão significativa do projeto de inventário, focada na comparação empírica de duas estruturas de dados fundamentais em C: Vetor (Lista Sequencial) e Lista Encadeada (Estrutura Dinâmica).

Funcionalidade Principal
Implementação Dupla: Todas as operações básicas de inventário (inserção, remoção, listagem) foram implementadas em paralelo para as duas estruturas.

Análise de Performance: Introdução de contadores para medir o número de comparações realizadas nas buscas, demonstrando a eficiência de cada método.

Busca Avançada: O Vetor agora suporta Ordenação (Bubble Sort) e Busca Binária, destacando a vantagem da ordenação em listas sequenciais

struct Item: Mantida para dados do objeto.

struct No: Nova estrutura que contém o Item e o ponteiro *proximo.

Contadores: Variáveis (comparacoesSequencial, comparacoesBinaria) para quantificar o trabalho de cada algoritmo de busca.

Gerenciamento de Memória: Implementação da função liberarLista() para desalocar todos os nós criados dinamicamente.

Este commit representa o estágio final do projeto de inventário/planejamento, onde o foco muda para a análise de desempenho de algoritmos de ordenação e a aplicação de Busca Binária para otimização estratégica.

Funcionalidade Principal
Priorização Estratégica: O jogador pode escolher entre diferentes algoritmos de ordenação para organizar os componentes de montagem da Torre de Fuga com base em critérios (Nome, Tipo, Prioridade).

Análise de Desempenho: O sistema mede e exibe o número de comparações e o tempo de execução (clock()) de cada algoritmo de ordenação, fornecendo feedback educacional sobre eficiência.

Ativação da Torre: Implementação da Busca Binária para localizar rapidamente o componente-chave (chip central), uma operação que só pode ser realizada após a ordenação do vetor por nome.

