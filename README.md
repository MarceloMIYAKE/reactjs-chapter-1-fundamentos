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