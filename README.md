# Composite Pattern
## Obejtivo
Utilizado para representar um objeto formado pela composição de objetos similares. Este conjunto de objetos pressupõe uma mesma hierarquia de classes a que ele pertence. Tal padrão é, normalmente, utilizado para representar listas recorrentes, ou recursivas, de elementos;
## Motivação
A intenção do padrão Composite é compor objetos em estruturas de árvore para representar hierarquia partes-todo;
## Aplicabilidade
Pode ser utilizado quando queremos trabalhar uma hierarquia de objetos que representem uma mesma super-classe, de modo a tornar sua operação padronizada, sendo, na maioria das vezes, em combinação com o padrão Iterator. Imagine um sistema de gerenciamento de arquivos.
Nesse sistema é possível criar arquivos concretos (vídeos, textos, imagens, etc.) e arquivos pastas, que armazenam outros arquivos. O problema é o mesmo, como fazer um design que atenda estes requerimentos? Através do padrão Composite, todos terão uma forma comum de serem reconhecidos e trabalhados, através de uma super-classe;
## Estrutura 
Abaixo, temos a estrutura UML do pattern, descrita no livro do GoF. Component declara a interface para objetos nessa composição, implementa o comportamento padrão para a interface comum à todas as classes e declara uma interface para acessar os componentes-filho. Leaf representa o objeto folha na composição. A folha não tem nenhum componente-filho, define o comportamento para objetos primitivos na composição e herda todos os métodos de Component, porém só implementa de fato os que lhe interessam – neste caso, o método Operation, nos outros são inseridos exceções que serão geradas em tempo de execução. Composite define o comportamento para componentes que possuam componentes-filho, armazena componentes-filho e implementa funções relacionadas aos componentes-filho na interface do Componente. E finalmente, Client opera os objetos da composição através da interface do Componente;
