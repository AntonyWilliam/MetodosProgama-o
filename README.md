Métodos Avançados de Programação
UNIESP Faculdades
Professora
Drª Alana Morais (alanamm.prof@gmail.com)
Aluno
Antony William Ramalho Vieira

Padrão Comportamental:
Iterator

Padrão Iterator
Problema:
Coleções são um grupo de containers de objetos, e na programação está cheio deles, 
organizando-os em listas simples, mas não importando como uma lista e feita deve ter uma forma de acessa-la
, acessando os elementos sem repeti-los, normalmente isso seria simples, simplesmente varrendo todos os elementos
, mas e se tivermos uma ordem mais sofisticada como em uma arvore, como por exemplo você pode querer ir de um galho a outro
, ou verificar as folhas em seguida e o tronco
, e esse o problema que este padrão procura solucionar.

Solução:
A ideia e extrair coleções em objetos separados chamados de iterator, quando implementamos o algoritmo ele encapsula todos os detalhes da travessia
, como por exemplo a posição atual de um elemento e quantos faltam para acabar a lista, por causa disso os iterators podem passar por várias coleções 
ao mesmo tempo, todos os iterators devem usar a mesma interface isso faz com que o código do cliente fique compatível com qualquer tipo de coleção.

Consequências:
Retira agregação e responsabilidade
Simplificando a interface e a sua implementação
Alta coesão com as classes

Exemplo:
Uma classe principal chamada menuItem que possui uma interface chamada interator que é implementada em outra classe chamada
Menu interator, que irá iterar uma coleção de menus, para percorrer os itens facilitando a interação com tudo.
