# Composite Pattern
## Obejtivo
Utilizado para representar um objeto formado pela composição de objetos similares. Este conjunto de objetos pressupõe uma mesma hierarquia de classes a que ele pertence. Tal padrão é, normalmente, utilizado para representar listas recorrentes, ou recursivas, de elementos;
## Motivação
A intenção do padrão Composite é compor objetos em estruturas de árvore para representar hierarquia partes-todo;
## Aplicabilidade
Pode ser utilizado quando queremos trabalhar uma hierarquia de objetos que representem uma mesma super-classe, de modo a tornar sua operação padronizada, sendo, na maioria das vezes, em combinação com o padrão Iterator. Imagine um sistema de gerenciamento de arquivos.
Nesse sistema é possível criar arquivos concretos (vídeos, textos, imagens, etc.) e arquivos pastas, que armazenam outros arquivos. O problema é o mesmo, como fazer um design que atenda estes requerimentos? Através do padrão Composite, todos terão uma forma comum de serem reconhecidos e trabalhados, através de uma super-classe;
## Estrutura 
![composite](https://user-images.githubusercontent.com/43156684/93627923-19308700-f9bc-11ea-8b6c-31108cf18c55.gif)
## Autor
Gustavo Hirata Kiyatake RA:1811514003
