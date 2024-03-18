# ALUNO
Flávio Henrique Simões Brito

# PROJETO
Esse projeto consiste no gerenciamento de uma biblioteca utilizando o Modelo Entidade-Relacionamento.

### REQUISITOS MÍNIMOS
- Entidade livro;
- Entidade autor;
- Entidade usuário;
- Empréstimo como relacionamento;
- Estabelecimento de cada relação feita, inclusive a de livro e autor
- Uso de cardinalidade;
- Especialização modeladas.

### REQUISITOS ADICIONAIS
- Setor(entidade), pois a biblioteca pode ser dividida em setores diferentes sendo diferenciadas por andar(chave) e curso, para melhor organização...
- Doa(relacionamento), pois o usuário pode doar um produto para a biblioteca...
- Faz compra(relacionamento), pois um produto ou mais pode estar à venda e o usuário pode comprá-lo, nele tem a chave que é código da compra, preço(atributo), forma de pagamento(atributo) e dependendo da forma de pagamento, pode ter uma taxa adicional(atributo de forma de pagamento).
- Sala(entidade), uma biblioteca pode ter várias salas para disponibilizar ao usuário de ler na biblioteca, caso queira
- Sala Premium(entidade), é uma especialização de sala, onde apenas assinantes podem ter acesso. Esse tipo de sala possui computadores(atributo) e projetor(atributo) para deixar o assinante mais confortável e ele continuar ajudando a biblioteca a ter mais lucro.
- 