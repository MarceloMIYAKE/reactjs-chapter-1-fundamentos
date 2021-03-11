# ReactJS
## Configurando ambiente
### Ambiente de desenvolvimento
- Node: https://github.com/nvm-sh/nvm#installing-and-updating
  - `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash`
  - ~/.zshrc
    ```
    export NVM_DIR="$HOME/.nvm"
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
    [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
    ```
  - `nvm install 14 --lts`
  - `nvm use 14`
- Yarn: https://yarnpkg.com/getting-started/install
  - `npm install --global yarn`
### Criando estrutura do projeto
- Inicialização do projeto
  ```
  yarn init -y
  ```
- React
  ```
  yarn add react
  ```
- ReactJS
  ```
  yarn add react-dom
  ```
- Diretórios `src` e `public`
  ```
  mkdir src public
  ```
### Configurando Babel
- Babel
  ```
  yarn add @babel/core @babel/cli @babel/preset-env @babel/preset-react -D
  ```
- Criar `babel.config.js`
- Teste: `yarn babel src/index.jsx --out-file dist/bundle.js`
### Configurando Webpack
- Webpack
  ```
  yarn add webpack webpack-cli -D
  ```
- Criar `webpack.config.js`
- Babel loader
  ```
  yarn add babel-loader -D
  ```
### Servindo HTML estático
- HTML Webpack Plugin
  ```
  yarn add html-webpack-plugin -D
  ```
### Webpack Dev Server
- Webpack Dev Server
  ```
  yarn add webpack-dev-server -D
  ```
- Executar
  ```
  yarn webpack serve
  ```
### Ambiente dev e produção
- Cross Env
  ```
  yarn add cross-env -D
  ```
- Executar em ambiente de dev
  ```
  yarn dev
  ```
- Executar em ambiente de produção
  ```
  yarn build
  ```
### Importante arquivos CSS
- Criar diretório `styles`
  ```
  mkdir src/styles
  ```
- Style loader & CSS loader
  ```
  yarn add style-loader css-loader -D
  ```
