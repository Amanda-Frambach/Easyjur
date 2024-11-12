# Projeto Easyjur

É um projeto solicitado com foco em testes de automação de login e crud em site e areas especificas fornecidas pela solicitante.

Os projetos manteram os mesmos nomes EasyJur para que seja de facil localização no Guthub e no Gitlab, então ao acessar deve clonar o projeto pelog gitlab,
Importante ressaltar que não utilizaremos actions,
Para utilizar esse projeto deve-se realizar a configuração abaixo:

Tecnologias utilizadas e suas configurações:

Cypress com linguaguem javascrip e formato de page object para os testes de web
    extensoes utilizadas no projeto: Material Icon, Dark One Pro e git graph:

1.Instalar Visual code studio;
ACesso o site code.visualstudio.com e realize o download na versão do seu Sistema Operacional Stable, mantenha a configuração padrão até finalizar
Adicione as extensões citadas

1.Instalar Node.js
Acesso o site nodejs.org.net e realize o download na versão do seu Sistema Operacional LTS, adicione a versão PATH e mantenha a configuração padrão até finalizar

1.Instalar Cypress
Acesso o diretorio do projeto pelo cmd
Crie uma pasta para o cypress e acesse a pasta
mkdir cypress
cd cypress

digite no cmd:
npm init

O Arquivo package.json será criado, colocaramos o cypress como dependencia no diretorio por boas praticas;
npm i cypress --save-dev

Após a instalação do cypress digite para abrir ainda no terminal para abrir;
npx cypress open

ESLINT para analise de código estatico via cmd

Para instalar o ESLint em um projeto JavaScript ou TypeScript, você pode seguir estes passos:

1. Preparação
Certifique-se de que o Node.js e o npm (ou yarn) estão instalados no sistema. Você pode verificar a instalação do Node.js com
node -v
e do npm com:
npm -v

2.Instalar o ESLint
No diretório do seu projeto, instale o ESLint como uma dependência de desenvolvimento:
npm install eslint --save-dev

3. Configurar o ESLint
Após instalar, você pode configurar o ESLint automaticamente com o comando:

npx eslint --init
Esse comando irá abrir um assistente para guiar a configuração do ESLint. Mantenha como a imagem abaixo:

Ok to proceed? (y) y


> npx
> create-config

@eslint/create-config: v1.4.0

√ How would you like to use ESLint? · problems
? What type of modules does your project use? ...
> JavaScript modules (import/export)
  CommonJS (require/exports)
√ What type of modules does your project use? · esm
√ Which framework does your project use? · none
√ Does your project use TypeScript? · javascript
√ Where does your code run? · browser
The config that you've selected requires the following dependencies:

Com base nas respostas, o ESLint cria um arquivo de configuração (.eslintrc.json, .eslintrc.yml ou .eslintrc.js) no diretório do seu projeto.

4. Adicionar Scripts para Facilitar a Execução (opcional)
No arquivo package.json, você pode adicionar um script para rodar o ESLint em seu código:
json
Copiar código
"scripts": {
  "lint": "eslint ."
}

5. Executar o ESLint
Agora, você pode rodar o ESLint para verificar seu código:
npm run lint

O ESLint analisará o código no diretório atual e reportará problemas de acordo com as regras definidas na configuração.

7.  Corrigir Problemas Automaticamente
Para corrigir automaticamente problemas de formatação e alguns erros, você pode usar o flag --fix:
npx eslint . --fix
