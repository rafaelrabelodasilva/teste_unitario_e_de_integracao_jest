# O projeto 🧙

Este projeto foi criado como exercício do curso "Node.js: testes unitários e de integração".<br>
Nele criei testes unitários com o jest.<br>
Criei um arquivo chamado "assercoes.js" que contém alguns exemplos de asserções. Também criei o arquivo index com algumas funções que exportei para serem usadas nos testes que estão dentro da pasta "test".<br>
- O teste "operacoes" foi uma busca que fiz no jestjs.io para entender melhor o que essa ferramenta é capaz.
- O teste "folhaDePagamento" e carrinho são testes que aprendi com o curso da Alura que ainda não foi finalizado.

## Dependências

Neste projeto adicionamos o **Jest** que é um framework de teste unitário. Para instalar-lo basta digitar o comando abaixo no terminal:<br>

`npm install --save-dev jest`

Também adicionamos o **Eslint** que é uma ferramenta que analisa o código e aponta quaisquer problemas que encontrar. Ele pode encontrar bugs, áreas potencialmente problemáticas, estilos de codificação ruins e questões de estilo. Para instalar-lo basta digitar o comando abaixo no terminal:<br>

`npm install --save-dev eslint`

## Observações

Para executar os testes e exibir o relatório de testes simples basta digitar o comando abaixo no terminal:<br>

`npm run test`

![gif](./imagens/npm-run-test.gif "npm run test")

Para ficar assistindo o código e rodar automaticamente os testes conforme as alterações são feitas e salvas no projeto digitar o comando abaixo no terminal:<br>

`npm run test:watch`

![gif](./imagens/npm-run-test-watch.gif "npm run test:watch")

Para exibir o relatório de testes em forma de tabela (ferramenta integrada do jest para cobertura de testes, que possibilita identificar caminhos não testados no código):<br>

`npm run test:coverage`

![gif](./imagens/npm-run-test-coverage.gif "npm run test coverage")

Colunas da tabela acima e suas explicações:

- File: indica quais arquivos de teste do diretório estão sendo executados. Cada linha dessa coluna fornece as estatísticas para cada arquivo de teste localizado e executado pelo Jest.

- Stmts: lista a porcentagem de statements do código que foram cobertos pelos testes. Em programação, um statement (ou declaração) é cada comando individual que damos ao programa para que ele execute instruções.

- Branch: exibe em quais arquivos há ramificações que precisam ter todas as suas condições testadas. Embora tenham o mesmo nome, não confundir estas branches com branches de versionamento do Git. O Jest não acessa o repositório do Git e nem há nenhum teste a ser feito nesse sentido.

- Funcs: exibe qual a porcentagem de funções presentes em cada arquivo que foram executadas/chamadas pelos testes.

- Lines: exibe a porcentagem de linhas de código por onde os testes passaram durante a sua execução. Quando está em 100%, significa que os testes percorreram todas as linhas de código dos arquivos testados. Quando não está em 100%, devemos observar a coluna seguinte (Uncovered Lines), que vai indicar por quais linhas o Jest não passou ao executar os testes nos arquivos.

- Uncovered lines: exibe quais linhas de cada arquivo não foram percorridas pelo Jest.

**Dica:**<br>
O Jest também fornece o relatório de cobertura de forma mais visual. Quando utilizamos a flag coverage, além de exibir o relatório no terminal, o Jest também cria a pasta coverage na raiz do projeto. Dentro desta pasta, você pode acessar a subpasta lcov-report para ver o relatório (report) e interagir com os arquivos, abrindo o arquivo index.html e navegando pelos arquivos.