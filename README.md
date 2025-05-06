# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas seguintes linguagens: Python, JavaScript, TypeScript e Java.

Você deve submeter via Moodle apenas o link do seu `fork`, conforme descrito abaixo.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
pip install gitevo
```

Rode a ferramenta no repositório selecionado através do seguinte comando (dependendo da linguagem do projeto que escolheu):

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r js <git_url>

# TypeScript
$ gitevo -r ts <git_url>

# Java
$ gitevo -r java <git_url>
```

Onde `<git_url>` é URL do repositório a ser analisado.
Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

# Passo 3: Explorar os gráficos de evolução de código (`index.html`)

Ao rodar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), o arquivo `index.html` é gerado com diversos gráficos de evolução de código.

Abra o arquivo `index.html` e observe com atenção os gráficos gerados.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo, 
- Detalhar se as curvas estão de acordo com boas práticas,
- Explicar grandes alterações nas curvas,
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- Etc.

Seja criativo!

# Exercício

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: https://github.com/expressjs/express

2. Gráfico selecionado: JavaScript files
  
3. Explicação: o gráfico ostra a evolução da quantidade de arquivos JavaScript no repositório do Express, um dos frameworks mais utilizados para aplicações web em Node.js. Observando a curva, nota-se que entre os anos de 2020 e 2025 a quantidade de arquivos se manteve praticamente estável, sempre em torno de 150 a 155 arquivos. Isso indica que o projeto vinha sendo mantido de forma madura e consistente, sem grandes expansões ou inchaços desnecessários no código. Essa estabilidade é, inclusive, um bom sinal: mostra que a equipe do Express tem seguido boas práticas de modularização e manutenção. No entanto, em 2025 houve uma queda mais acentuada, reduzindo o número de arquivos para cerca de 140. Existem algumas hipóteses para essa queda: pode ter havido uma limpeza de código legado, uma reorganização dos módulos internos para torná-los mais concisos, ou até uma migração parcial para TypeScript, algo que vem se tornando comum em muitos projetos open source nos últimos anos. Outra possibilidade é que algumas funcionalidades menos essenciais tenham sido extraídas do núcleo do Express e movidas para bibliotecas separadas. De qualquer forma, essa queda não representa um problema, e sim uma provável ação de refatoração bem pensada. 



