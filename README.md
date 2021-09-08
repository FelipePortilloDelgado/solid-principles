## SOLID

#### 5 princípios

Os 5 princípios de desenvolvimento de software servem como diretrizes para deixar o sistema mais flexível, menos rígido, menos frágil, mais fácil de manter e evoluir.

##### S - SRP

Single Responsibility Principle

Quando a classe possui muitas responsabilidades, há um aumento na possibilidades de ocorrerem bugs em decorrência de suas mudanças, que podem afetar até outras partes do sistema sem você saber.
O objetivo principal da responsabilidade única, é isolar essas responsabilidades para caso ocorra um bug com suas alterações, não afete as outras partes do sistema.

<img src="https://miro.medium.com/max/2000/1*P3oONz9Da3Tc1w97fMV73Q.png" alt="SRP">
<a href="https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898" target="_blank">Fonte: [Imagem 1] https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898</a><br/><br/>

- Separar coisas que MUDAM POR MOTIVOS DIFERENTES
- Mover responsabilidades

##### O - OCP

Open Closed Principle

Este principio tem como principal objetivo extender o comportamento de uma classe, e não modificar os comportamentos já existentes, podendo afetar todo o sistema que depende dessa classe.

<img src="https://miro.medium.com/max/2000/1*0MtFBmm6L2WVM04qCJOZPQ.png" alt="OCP">
<a href="https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898" target="_blank">Fonte: [Imagem 2] https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898</a><br/><br/>


- Devemos estar fechados para modificação e abertos para extensão

##### L - LSP

Liskov Substitution Principle

O principal objetivo da substituição de liskov é padronizar o comportamento entre classes pais e filhos, as classes devem ser capaz de processar os mesmo requests e entregar os mesmos resultados, podendo substituir uma pela outra sem causar nenhum erro no sistema.

<img src="https://miro.medium.com/max/2000/1*yKk2XKJaCLNlDxQMx1r55Q.png" alt="OCP">
<a href="https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898" target="_blank">Fonte: [Imagem 3] https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898</a><br/><br/>

- Se S (Beer, Whisky, Water) é subclasse de T (Item), em um programa deve ser possível substituir instâncias de T (Item) por instâncias de S (Beer, Whisky, Water), SEM QUEBRAR O FUNCIONAMENTO DO PROGRAMA

- Pré-condições não podem ser fortalecidas
  - Deixando de aceitar ENTRADAS que a superclasse considera válida

- Pós-condições não podem ser enfraquecidas
  - Aceitando saídas mais AMPLAS

- Invariantes devem se manter consistentes
  - Se uma subclasse permitir que o estado conceitual da hierarquia de classes fique inválido

##### I - ISP

Interface Segregation Principle

O principal objetivo do principio da segregação de interface é a não obrigatoriedade de implementar comportamentos que não serão usados pela classe.

<img src="https://miro.medium.com/max/5200/1*2hmyR9L43Vm64MYxj4Y89w.png" alt="OCP">
<a href="https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898" target="_blank">Fonte: [Imagem 4] https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898</a><br/><br/>

- Cuidado com interfaces MUITO ABRANGENTES, não obrigue subclasses a implementar métodos que elas não precisam

##### D - DIP

Dependency Inversion Principle

O principal objetivo do principio de inversão de dependência é fazer com que classes de alto nível não execute códigos de classes de baixo nível, ao invés disso fornecer uma interface para essa iteração.

<img src="https://miro.medium.com/max/2000/1*Qk8tDmjQlyvwKxNTfXIo0Q.png" alt="OCP">
<a href="https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898" target="_blank">Fonte: [Imagem 5] https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898</a><br/><br/>

- High-level modules should not depend on low-level modules
Both should depend on abstractions


