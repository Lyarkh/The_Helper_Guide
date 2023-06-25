
## Resumo
---
O conceito de MVC (Model-View-Controller) é um padrão de arquitetura de software amplamente utilizado no desenvolvimento de aplicativos. Ele divide uma aplicação em três componentes principais: o Modelo (Model), a Visão (View) e o Controlador (Controller). Cada componente tem uma função específica e trabalha em conjunto para fornecer uma separação clara de responsabilidades e melhorar a manutenção e escalabilidade do código.


## Principais  Características
---
1. **Modelo (Model):** O Modelo representa a lógica de negócios da aplicação e os dados subjacentes. Ele encapsula a manipulação, validação e recuperação dos dados, além de fornecer métodos para interagir com eles. O Modelo não tem conhecimento sobre a interface do usuário ou a forma como os dados são apresentados.
    
2. **Visão (View):** A Visão é responsável por apresentar os dados ao usuário e lidar com a interação do usuário. Ela exibe a informação de maneira visualmente agradável e compreensível. A Visão não possui lógica de negócios, apenas mostra os dados fornecidos pelo Modelo e envia eventos para o Controlador quando o usuário interage com ela.
    
3. **Controlador (Controller)**:  O Controlador atua como intermediário entre o Modelo e a Visão. Ele recebe as ações do usuário provenientes da Visão, processa-as e interage com o Modelo, solicitando as operações adequadas. Ele também atualiza a Visão de acordo com as mudanças nos dados do Modelo.