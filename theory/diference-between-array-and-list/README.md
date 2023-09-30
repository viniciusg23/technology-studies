# Diferença entre Arrays e Listas Encadeadas
## O que é Array e Lista Encadeada
Arrays e listas encadeadas são elementos da programação que nos permitem armazenar conjuntos de dados. Ao contrário de uma variável simples que armazena apenas um valor, esses elementos podem armazenar vários valores diferentes de forma organizada.
## Como funciona a memória do computador
A memória do computador pode ser comparada a uma tabela do Excel ou a algum outro editor de planilhas. Existem várias células, cada uma com seu endereço único (coluna:linha) e o valor armazenado na célula. Sempre que algo precisa ser armazenado na memória do computador, o sistema solicita um local para isso, e ele fornece o endereço do espaço que pode ser usado.
## Diferença entre Array e Lista Encadeada
Quando é necessário armazenar um conjunto de elementos na memória, é preciso escolher entre esses dois tipos, e a diferença entre eles é a seguinte:
### Array
Um array armazena todos os itens consecutivamente na memória. 
![](./image1.png)
No entanto, no exemplo acima para adicionar um novo elemento ao array, é necessário movê-lo para outro local, pois o próximo espaço de memória já está sendo utilizado, e todos os elementos de um array devem estar **um ao lado do outro** na memória. 
É possível reservar uma quantidade específica de espaço de memória ao criar um vetor para evitar a realocação de todo o vetor, o que consome poder de processamento. No entanto, isso cria um dilema:
- Nem todos os espaços do vetor podem ser utilizados, resultando em memória não utilizada.
- A quantidade de elementos pode exceder o limite do vetor, exigindo a realocação de qualquer maneira.
### Listas Encadeadas
Os elementos das listas são armazenados dinamicamente na memória, ou seja, um novo item pode ser adicionado em qualquer "buraco" na memória. Cada item na lista armazena seu valor e o endereço do próximo item, conectando assim todos os itens em um conjunto.
![](./image2.png)
Para inserir um novo elemento na lista, basta armazenar o endereço de memória do novo item em algum outro elemento já existente na lista.
## Inserção e Deleção de elementos
Em sistemas, dados diferentes são adicionados e removidos constantemente. Para isso, tanto arrays quanto listas têm funcionalidades diferentes.
### Array
Inserir ou remover um elemento de um array tem uma complexidade linear. Por exemplo, ao remover um item do array, todos os itens à frente dele devem ser "arrastados" para trás para evitar espaços vazios no meio. Da mesma forma, ao inserir algo no meio do conjunto, todos os outros elementos devem ser "empurrados" para frente.
### Listas Encadeadas
Inserir ou remover um elemento de uma lista tem uma complexidade constante. Por exemplo, ao remover um item do meio da lista, basta alterar o endereço que o elemento anterior referencia para o endereço que o item a ser removido está referenciando. Dessa forma, o "buraco" é preenchido com apenas esse pequeno ajuste.
![](./image3.png)
## Acesso aos elementos
Esses dados são armazenados para serem acessados posteriormente, e arrays e listas também diferem no acesso aos elementos.
### Array
Acessar um elemento aleatório em um array tem complexidade constante. Com apenas uma operação, é possível acessar qualquer item do conjunto, pois o computador sabe que todos os elementos estão um ao lado do outro. Se for solicitado o item na posição 10, o computador pode pular diretamente para o 10º elemento a partir do endereço de início do array.
### Listas Encadeadas
Acessar um elemento aleatório em uma lista tem complexidade linear. O computador precisa passar por item por item para encontrar o desejado, pois os itens foram armazenados de forma aleatória na memória, e só é possível acessar um elemento da lista a partir do endereço armazenado no elemento anterior.
## Referência
Bhargava, Aditya Y. 2017. Entendendo Algoritmos. Editora Novatec.