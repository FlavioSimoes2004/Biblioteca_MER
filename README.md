# ALUNO
Flávio Henrique Simões Brito

# PROJETO
Esse projeto consiste no gerenciamento de uma biblioteca conceitual utilizando o Modelo Entidade-Relacionamento.

### REQUISITOS MÍNIMOS
- Entidade livro;
- Entidade autor;
- Entidade usuário;
- Empréstimo;
- Estabelecimento de cada relação feita, inclusive a de livro e autor
- Uso de cardinalidade;
- Especializações modeladas.

### REQUISITOS ADICIONAIS
- Setor(entidade), pois a biblioteca pode ser dividida em setores diferentes sendo diferenciadas por andar(chave) e curso(atributo), para melhor organização.
- Produto(entidade), tem escializações, o produto é o que se pode pegar emprestado, comprar ou doar para a biblioteca. Ele tem a chave código produto e atributos disponibilidade, para saber se está disponível para ser comprado ou emprestado, título, caso o usuário esteja procurando por um produto, ele vai pesquisar pelo título, e está a venda, para dizer que há a possibilidade de compra do produto. Um ou mais produtos podem ter um ou mais autores.
- Ebook(entidade), especialização de produto, ele tem PDFs e livros dentro. Essa entidade acrescenta mais opções de produto aos usuários.
- DVD(entidade), especialização de produto, tem como atributos a produtora do vídeo/filme/documentário e o diretor. Essa entidade acrescenta mais opções de produto aos usuários.
- Doa(relacionamento), pois um usuário pode doar um ou muitos produtos para a biblioteca.
- Faz compra(relacionamento), pois um usuário pode comprar um ou muitos produtos se estiver a venda, nele tem a chave que é código da compra, preço(atributo), forma de pagamento(atributo) e dependendo da forma de pagamento, pode ter uma taxa adicional(atributo).
- Sala(entidade), uma biblioteca pode ter várias salas para disponibilizar ao usuário de ler na biblioteca, caso queira. Nela tem a chave que é o número da sala e há atributos como disponibilidade, para saber se a sala está ocupada.
- Sala Premium(entidade), é uma especialização de sala, onde apenas assinantes podem ter acesso. Esse tipo de sala possui computadores(atributo) e projetor(atributo) para deixar o assinante mais confortável e ele continuar ajudando a biblioteca financeiramente.
- Assinante(entidade), é uma especialização de usuário, ele contribui financeiramente com a biblioteca, e por isso, ele tem descontos em compras e multas(atributo) e ganha acesso à salas premium.
- Funcionário(entidade), é uma especialização de usuário, pois o funcionário também pode pegar emprestado, comprar ou doar para a biblioteca. Ele trabalha para a biblioteca e ajuda os usuário a encontrarem os produtos.
- Gerente(entidade), faz parte da especialização funcionário, tem como atributo o setor que ele é responsável por gerenciar.