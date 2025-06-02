<h1> <b> Clean Code </b> </h1>

Exemplos e trechos retirados do livro <i>Clean Code</i>, de <i>Robert C. Martin</i> para o aperfeiçoamento de um código limpo.

<h2> <b> 0. A Regra do Escoteiro </b> </h2>
"Não basta escrever um código bom. Ele precisa ser mantido sempre limpo. Todos já vimos códigos estragarem e degradarem com o tempo, portanto, precisamos assumir um papel ativo na prevenção da degradação. A Boy Scouts of America, maior organização de jovens escoteiros dos EUA, tem uma regra simples que poremos aplicar a nossa profissão:
Deixe a área do acampamento mais limpa do que como você a encontrou."

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

<h2> <b> 3. Comentários </b> </h2>

"O uso adequado de comentários é compensar nosso fracasso em nos expressar no código. Comentários são sempre fracassos. Devemos usá-los porque nem sempre encontramos uma forma de nos expressar sem eles, mas seu uso não é motivo de comemoração."

<h3> <b> 3.1 Comentários Compensam um Código Ruim </b> </h3>

"Códigos claros e expressivos com poucos comentários são de longe superiores a um amontoado e complexo com muitos comentários. Ao invés de gastar seu tempo criando comentários para explicar a bagunça que você fez, use-o para limpar essa zona."

<h3> <b> 3.2 Explique-se no código </b> </h3>

"O que você preferiria ver? Isso:"
```
//Verifica se o funcionário tem direito a todos os benefícios
if ((employee.flags & HOURLY_FLAG) && (employee.age > 65))
```
"Ou isso?"
```
if (employee.isEligibleForFullBenefits())
```

<h3> <b> 3.3 Alertas Sobre Consequências </b> </h3>

"Às vezes é útil alertar outros programadores sobre certas consequências."

<h3> <b> 3.4 Destaque </b> </h3>

"Pode-se usar um comentário para destacar a importância de algo que talvez pareça irrelevante."

<h3> <b> 3.5 Cabeçalhos de Funções </b> </h3>

"Funções curtas não requerem muita explicação. Um nome bem selecionado para uma função pequena que faça apenas uma coisa costuma ser melhor do que um comentário no cabeçalho."

<h2> <b> 4. Formatação </b> </h2>

<h3> <b> 4.1 Formatação Vertical </b> </h3>

"O seu código-fonte deve ser de que tamanho? A partir de códigos simples de 200 linhas, com um limite máximo de 500 linhas. Embora essa não deva ser uma regra fixa, deve-se considerá-la bastante, pois arquivos pequenos costumam ser mais fáceis de se entender do que os grandes."

<h3> <b> 4.2 Espaçamento vertical entre conceitos </b> </h3>

"Cada linha representa uma expressão um uma estrutura, e cada grupo de linhas representa um pensamento completo. Esses pensamentos devem ficar separados por linhas em branco. Há linhas em branco que separam a declaração e a importação de pacotes e cada uma das funções. Essa simples e extrema regra tem grande impacto no layout visual do código."

<h3> <b> 4.3 Distância vertical </b> </h3>

4.3.1 "Os conceitos intimamente relacionados devem ficar juntos verticalmente." </br>
4.3.2 <b> Variáveis: </b> "Devem-se declarar as variáveis o mais próximo possível de onde serão usadas." </br>
4.3.3 <b> Variáveis de Instância: </b> "Devem-se declarar as variáveis de instância no início da classe." </br>
4.3.4 <b> Funções Dependentes: </b> "Se uma função chama outra, elas devem ficar verticalmente próximas, e a que chamar deve ficar acima da que for chamada." </br>
4.3.5 <b> Afinidade conceitual: </b> "Há outras causas possíveis de afinidade, que pode ser causada por um grupo de funções que efetuam uma operação parecida."

<h3> <b> 4.4 Formatação horizontal </b> </h3>

"Qual deve ser o tamanho de uma linha ? Os programadores claramente preferem linhas curtas. Eu, pessoalmente determinei 120 como meu limite."

<h2> <b> 5. Classes </b> </h2>

<h3> <b> 5.1 Organização das Classes </b> </h3>

"Uma classe deve começar com uma lista de variáveis. As públicas, estáticas e constantes, se existirem, devem vir primeiro. Depois vem as variáveis estáticas privadas, seguidas pelas instâncias privadas. Raramente há uma boa razão para se ter uma variável pública."

<h3> <b> 5.2 As classes devem ser pequenas! </b> </h3>

"Com as classes, contamos as responsabilidades. O nome de uma classe deve descrever quais responsabilidades ela faz. Devemos também poder escrever com cerca de 25 palavras uma breve descrição da classe."

<h3> <b> 5.3 O Princípio da Responsabilidade Única </b> </h3>

"O Princípio da Responsabilidade Única afirma que uma classe ou módulo deve ter um, e apenas um, motivo para mudar. Este princípio nos dá uma definição de responsabilidade e uma orientação para o tamanho da classe. Estas devem ter apenas uma responsabilidade e um motivo para mudar."
