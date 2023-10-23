`tags:` #devops #ci_cd 

## Resumo:

CI/CD é a abreviação de _Continuous Integration/Continuous Delivery,_ traduzindo para o português: integração e entrega contínuas. Trata-se de uma prática de desenvolvimento de software que visa tornar a integração de código mais eficiente por meio de builds e testes automatizados. Com a abordagem CI/CD é possível entregar [aplicações](https://www.redhat.com/pt-br/topics/cloud-native-apps?percmp=7013a0000034e7YAAQ&cicd=32h281b) com mais frequência aos clientes. Para tanto, regras de [automação](https://www.redhat.com/pt-br/topics/automation?cicd=32h281b) são aplicadas nas etapas de [desenvolvimento de apps](https://www.redhat.com/pt-br/topics/devops/[[url-nid:307771;title:'article%20%7C%20why%20choose%20red%20hat%20for%20cloud-native%20development?%27])

## Diferença entre CI e CD

O acrônimo CI/CD tem alguns significados. "CI" sempre se refere à integração contínua, que é um processo de automação para desenvolvedores. Uma CI bem-sucedida é quando novas mudanças no código de uma aplicação são desenvolvidas, testadas e consolidadas regularmente em um repositório compartilhado. É a solução ideal para evitar conflitos entre ramificações quando muitas apps são desenvolvidas ao mesmo tempo.

"CD" se refere à entrega contínua e/ou à implantação contínua, conceitos relacionados e usados alternadamente às vezes. Em ambos os casos, trata-se da automação de fases avançadas do pipeline. Porém, são usados às vezes separadamente para ilustrar o nível de automação presente.

![ci_cd](https://www.redhat.com/rhdc/managed-files/styles/wysiwyg_full_width/private/ci-cd-flow-desktop.png?itok=NNRD1Zj0)


## Integração Contínua

No desenvolvimento moderno de aplicações, o objetivo é que muitos desenvolvedores trabalhem ao mesmo tempo em diferentes funcionalidades na mesma app. No entanto, se uma organização tiver que consolidar todo o código-fonte de ramificação em apenas um dia (conhecido como "merge day" ou "dia de consolidação"), o trabalho poderá ser entediante, manual e demorado.

Com a integração contínua (CI), a equipe consolida as mudanças no código de volta a uma ramificação compartilhada (ou "tronco") com mais frequência (às vezes, até diariamente). As mudanças são consolidadas e depois validadas através da criação automática da aplicação. Vários testes automatizados, geralmente de unidade e integração, são feitos para garantir que as mudanças não corrompam a aplicação. Basicamente, tudo é testado, incluindo classes, funções e diferentes módulos que formam toda a aplicação. Em caso de conflito entre os códigos novos e existentes, a CI facilita a correção desses bugs com rapidez e frequência.


## Entrega contínua

Após a automação de compilações e dos testes de integração e unidade na CI, a entrega contínua automatiza o lançamento desse código validado em um repositório. Portanto, para ter um processo eficaz de entrega contínua, é importante que a CI já esteja integrada ao pipeline de desenvolvimento. O objetivo da entrega contínua é fazer com que a base de códigos esteja sempre pronta para implantação em um ambiente de produção.

Cada etapa da entrega contínua, desde a consolidação das mudanças de código até a entrega de compilações prontas para produção, inclui a automação do lançamento de códigos e de teste. No final desse processo, a equipe de operação pode implantar uma app no ambiente de produção com rapidez e facilidade.


## Implantação contínua

A etapa final de um pipeline de CI/CD sólido é a implantação contínua. Ela é um complemento da entrega contínua, que automatiza o lançamento de versões prontas para produção em um repositório de códigos. A implantação contínua automatiza o lançamento de uma app para a produção. Como não há um canal manual na etapa do pipeline antes da produção, a CI depende muito da automação otimizada dos testes.