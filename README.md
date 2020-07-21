<h1> <b> Clean Code </b> </h1>

Exemplos e trechos retirados do livro <i>Clean Code</i>, de <i>Robert C. Martin</i> para o aperfeiçoamento de um código limpo.

<h2> <b> 1. Nomes Significativos </b> </h2>

<h3> <b> 1.1 Use Nomes que Revelem seu Propósito </b> </h3>

"O nome de uma variável, função ou classe deve responder a todas as grandes questões. Ele deve lhe dizer porque existe, o que faz e como é usado. Se um nome requer um comentário, então ele não revela seu propósito."

<h3> <b> 1.2 Evite Informações Erradas </b> </h3>

1.2.1 "Os programadores devem evitar passar dicas falsas que confundem o sentido do código. Devemos evitar palavras cujos significados podem se desviar daquele que desejamos."</br>
1.2.2 "Não se refira a um grupo de contas como <i>accountList</i>, a menos que realmente seja uma <i>List</i>. A palavra list significa algo específico para programadores."</br>
1.2.3 "Cuidado ao usar nomes muito parecidos. Fica difícil perceber a pequena diferença entre um e outro."</br>

<h3> <b> 1.3 Use Nomes Pronunciáveis </b> </h3>

"Crie nomes pronunciáveis, se não puder pronunciar, não terá como discutir sobre tal nome sem parecer um idiota. Isso importa porque a programação é uma atividade social."

<h3> <b> 1.4 Nomes de Classes </b> </h3>

"Classes e objetos devem ter nomes com substantivo(s), como Cliente e Conta. Evite palavras como Processador, Dados ou Info no nome de uma classe, que também não deve ser um verbo."

<h3> <b> 1.5 Nomes de Métodos </b> </h3>

"Os nomes de métodos devem ter verbos. Devem-se nomear métodos de acesso, alteração e autenticação segundo seus valores e adicionar os prefixos get, set ou is."

<h2> <b> 2. Funções </b> </h2>

<h3> <b> 2.1 Pequenas! </b> </h3>

"A primeira regra para funções é que elas devem ser pequenas. As funções devem ter no máximo 20 linhas."

<h3> <b> 2.2 Blocos e Indentação </b> </h3>

"Blocos dentro de instruções if, else, while e outros devem ter apenas uma linha. Possívelmente uma chamada de função. O nível de indentação de uma função deve ser de, no máximo, um ou dois."

<h3> <b> 2.3 Faça Apenas uma Coisa </b> </h3>

"As funções devem fazer uma coisa. Devem fazê-la bem. Devem fazer apenas ela."

<h3> <b> 2.4 Parâmetros de Funções </b> </h3>

"A quantidade ideal de parâmetros é zero. Depois vem um, seguido de dois. Sempre que possível devem-se evitar três parâmetros"

<h3> <b> 2.5 Extraia os blocos try/catch </b> </h3>

"Esses blocos são feios por si só. Eles confundem a estrutura do código e misturam o tratamento de erro com o processamento normal do código. Portanto, é melhor colocar as estruturas em suas próprias funções"
