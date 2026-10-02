# Fokus

O **Fokus** é um projeto desenvolvido durante a formação **React Native: desenvolvendo com Expo**, da [Alura](https://www.alura.com.br/), plataforma brasileira de cursos online de tecnologia. Ao longo das aulas, este projeto será usado para aprender, na prática, como criar aplicações mobile com **React Native** e executar o desenvolvimento com o **Expo**.

Este README acompanha a evolução do projeto commit a commit, em uma ordem progressiva. Assim, cada etapa mostra o que foi construído e qual conceito começou a ser praticado.

## Como executar

Antes de começar, é necessário ter o [Node.js](https://nodejs.org/) instalado.

1. Instale as dependências:

   ```bash
   npm install
   ```

2. Inicie o servidor do Expo:

   ```bash
   npx expo start
   ```

3. Abra o aplicativo em uma das opções exibidas pelo Expo:
   - **Expo Go**, usando um dispositivo físico;
   - emulador Android;
   - simulador iOS;
   - navegador, usando `npm run web`.

O Expo Router utiliza rotas baseadas em arquivos. Por isso, a tela principal deste projeto está em `src/app/index.jsx`.

## Evolução por commit

### 1. Estrutura inicial do projeto — `571d9db` (`Initial commit`)

O primeiro commit cria a base completa do aplicativo a partir do template do Expo. Nesta etapa foram adicionados:

- a configuração do Expo em `app.json`;
- o `package.json` e o `package-lock.json`, responsáveis pelas dependências;
- a configuração do TypeScript;
- a estrutura inicial do Expo Router;
- componentes reutilizáveis, temas, hooks e estilos globais do template;
- imagens, ícones e demais recursos visuais;
- scripts auxiliares, como o `reset-project.js`.

Esse ponto de partida já permite executar o aplicativo e conhecer a organização de um projeto React Native multiplataforma. A maior parte do código ainda é a demonstração gerada automaticamente pelo Expo.

### 2. Limpeza do template e criação da tela de entrada — `4231803` (`init`)

O segundo commit prepara o projeto para receber a implementação do Fokus. O conteúdo de demonstração foi removido, incluindo componentes, tela de exploração, tema e hooks que não seriam usados imediatamente.

No lugar da tela TypeScript original, foi criada `src/app/index.jsx`, usando JavaScript com JSX. Ela apresenta uma estrutura mínima de React Native:

- `View` funciona como o contêiner da tela;
- `Text` exibe o conteúdo textual;
- `StyleSheet.create` organiza os estilos;
- `flex`, `alignItems` e `justifyContent` centralizam o conteúdo.

O aplicativo ficou mais simples e passou a ter uma base direta para as próximas aulas.

### 3. Primeiro conteúdo da aplicação — `19a23c4` (`Hello World`)

Neste commit, o texto automático do template foi substituído por **“Hello, World!”**. É uma alteração pequena, mas importante: a tela deixa de ser apenas uma confirmação de que o Expo está funcionando e passa a exibir o primeiro conteúdo definido para o Fokus.

Essa etapa reforça o fluxo básico de desenvolvimento: editar o arquivo da rota principal, salvar e observar a atualização da aplicação no ambiente do Expo.

### 4. Identidade visual inicial e qualidade do código — `33ecd0c` (`chore: update dependencies and add ESLint configuration`)

O estado atual acrescenta conteúdo e organização visual à tela inicial:

- título **“Hello, World!”** com tamanho maior e destaque;
- mensagem **“Welcome to Fokus!”** como texto complementar;
- fundo azul-escuro e textos claros;
- estilos separados para o contêiner, o título e o texto;
- margem entre os elementos para melhorar a leitura.

Também foi configurado o ESLint, ferramenta que ajuda a encontrar problemas de sintaxe e inconsistências no código. O arquivo `eslint.config.js` usa as regras recomendadas pelo Expo, e as dependências `eslint` e `eslint-config-expo` foram adicionadas ao projeto.

Para verificar o código, execute:

```bash
npm run lint
```

## Próximos passos

A base da aplicação está pronta para evoluir. Nas próximas etapas, o projeto poderá ganhar a interface e as funcionalidades centrais do Fokus, enquanto os conceitos de componentes, estilos, estado, interação e navegação forem apresentados na formação.

## Referências

- [Documentação do Expo](https://docs.expo.dev/)
- [Documentação do React Native](https://reactnative.dev/docs/getting-started)
- [Expo Router](https://docs.expo.dev/router/introduction/)
- [Formação da Alura](https://www.alura.com.br/formacao-react-native)
