# ALUNO
Flávio Henrique Simões Brito

# PROJETO
Esse projeto consiste no gerenciamento de uma biblioteca conceitual utilizando o Modelo Entidade-Relacionamento.

### REQUISITOS MÍNIMOS
- Entidade livro;
- Entidade autor, tem como chave o nome, pois um usuário pode procurar por um produto do autor sem conhecimento do título;
- Entidade usuário;
- Empréstimo como relacionamento;
- Estabelecimento de cada relação feita, inclusive a de livro e autor
- Uso de cardinalidade;
- Especialização modeladas.

### REQUISITOS ADICIONAIS
- Setor(entidade), pois a biblioteca pode ser dividida em setores diferentes sendo diferenciadas por andar(chave) e curso(atributo), para melhor organização.
- Produto(entidade), tem escializações, o produto é o que se pode pegar emprestado, comprar ou doar para a biblioteca. Ele tem a chave código produto e atributos disponibilidade, para saber se está disponível para ser comprado ou emprestado, título, caso o usuário esteja procurando por um produto, ele vai pesquisar pelo título, e está a venda, para dizer que há a possibilidade de compra do produto. Um ou mais produtos podem ter um ou mais autores.
- Doa(relacionamento), pois o usuário pode doar nenhum ou muitos produtos para a biblioteca.
- Faz compra(relacionamento), pois um usuário pode comprar nenhum ou muitos produtos se estiver a venda, nele tem a chave que é código da compra, preço(atributo), forma de pagamento(atributo) e dependendo da forma de pagamento, pode ter uma taxa adicional(atributo de forma de pagamento).
- Sala(entidade), uma biblioteca pode ter várias salas para disponibilizar ao usuário de ler na biblioteca, caso queira. Nela tem a chave que é o número da sala e há atributos como disponibilidade, para saber se a sala está ocupada.
- Sala Premium(entidade), é uma especialização de sala, onde apenas assinantes podem ter acesso. Esse tipo de sala possui computadores(atributo) e projetor(atributo) para deixar o assinante mais confortável e ele continuar ajudando a biblioteca financeiramente.