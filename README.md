# Projeto de implementação de uma árvore trie existencial para busca de títulos de filmes
Detalhes do projeto:
Este trabalho implementa uma trie existencial em linguagem C para armazenar e buscar titulos de filmes. Uma trie é uma estrutura de dados eficiente para armazenar strings e realizar buscas rápidas por prefixo, onde cada nó representa um caracter de um título de filme.
O programa lê os titulos de um arquivo chamado filmes.txt, padroniza-os e os insere na árvore. Em seguida, ele vai processar as consultas, que podem ser:
p prefixo: lista todos os filmes que possuem o prefixo no título;
l título: o mais longo prefixo do título que seja um nome de filme;
c padrão: lista todos os filmes cujos títulos casam com o padrão.

Dificuldades de implementação:
A implementação da busca com curingas foi complexa, tendo que explorar recursivamente a árvore e considerar todas as combinações possíveis. 
Outra dificuldade foi garantir a padronização correta dos títulos, fazendo a conversão dos caracteres especiais.

Para permitir que uma chave possa ser prefixo de outra, a trie utiliza o caracter nulo (\0) como marcador de fim de palavra. Quando um título é inserido, um nó adicional é criado para representar o caracter nulo, isso permite que a trie diferencie um prefixo e uma palavra completa.
