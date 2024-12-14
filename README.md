## 🌐 [English Version of README](README_EN.md)

# Nearby

Nearby é um aplicativo desenvolvido em React Native usando Expo Router. O objetivo é oferecer uma experiência que permita aos usuários explorar e ativar cupons em locais parceiros próximos. O app integra mapas interativos, categorias e detalhamento de locais com cupons disponíveis.

## 🔨 Funcionalidades do Projeto

- Visualização de estabelecimentos próximos em um mapa interativo.
- Navegação entre categorias de locais.
- Resgate de cupons via QR Code.
- Detalhamento de locais com informações como endereço, telefone e cupons disponíveis.
- Regulamentos para utilização de cupons.

### Exemplo Visual do Projeto

Adicione aqui capturas de tela ou GIFs do aplicativo em funcionamento.

## ✔️ Técnicas e Tecnologias Utilizadas

- **React Native**
- **Expo Router** para navegação.
- **Axios** para consumo de API.
- **Tabler Icons** para ícones personalizados.
- **Expo Camera** para leitura de QR Codes.
- **React Native Maps** para renderização do mapa interativo.
- **Prisma** como ORM para gerenciamento do banco de dados.
- **SQLite** como banco de dados local para desenvolvimento.

## 📁 Estrutura do Projeto

- **assets/**
    - **images/**: Contém ícones e imagens como `splash.png` e `icon.png`.
    - Outros recursos gráficos do aplicativo.
- **api/**
    - **prisma/**: Contém os arquivos de configuração do banco de dados, incluindo o esquema e as migrações.
    - **src/**: Inclui os controladores, middlewares e servidor Express.
    - **seed.ts**: Script para popular o banco de dados com dados iniciais.
- **src/**
    - **app/**: Contém as rotas e telas principais do aplicativo.
    - **components/**: Componentes reutilizáveis, como botões, listas e mapas.
    - **services/**: Configuração de conexão com a API.
    - **styles/**: Arquivos de estilo global, como cores e famílias de fontes.
    - **utils/**: Funções auxiliares e ícones para categorias.

Exemplo detalhado:

- **src/app/home.tsx**: Tela inicial que exibe o mapa e os locais.
- **src/app/market/[id].tsx**: Tela de detalhes de um local.
- **src/components/button/**: Botões personalizados reutilizáveis.
- **src/styles/theme.ts**: Configurações de tema com cores e fontes.
- **api/seed.ts**: Script para popular o banco de dados com dados iniciais, como categorias, mercados e regras.

## 🛠️ Abrir e rodar o projeto

Para iniciar o projeto localmente, siga os passos abaixo:

1. **Certifique-se de que o Node.js está instalado**:
    - O [Node.js](https://nodejs.org/) é necessário para rodar o projeto. Você pode verificar se já o tem instalado com:
      ```bash
      node -v
      ```
    - Se não estiver instalado, baixe e instale a versão recomendada.

2. **Clone o Repositório**:
    - Copie a URL do repositório e execute o comando abaixo no terminal:
      ```bash
      git clone <URL_DO_REPOSITORIO>
      ```

3. **Instale as dependências**:
    - Navegue até o diretório do projeto e execute:
      ```bash
      npm install
      ```

4. **Configure e inicie o backend**:
    - Navegue para o diretório `api`:
      ```bash
      cd api
      ```
    - Gere o cliente Prisma necessário para o banco de dados:
      ```bash
      npx prisma generate
      ```
    - Execute o seguinte para iniciar o backend:
      ```bash
      npm run start
      ```

5. **Inicie o aplicativo mobile**:
    - Navegue para o diretório `mobile`:
      ```bash
      cd mobile
      ```
    - Execute o comando:
      ```bash
      npx expo start
      ```

6. **Acesse o aplicativo**:
    - Use o app Expo Go para escanear o QR Code gerado.
    - Ou rode o aplicativo em um emulador Android (e.g., Android Studio).

## 📚 Material de Apoio

- Documentação adicional: [Guia NLW Mobile](https://docs-rocketseat.notion.site/NLW-Mobile-149395da577080a398d5dde2d90321ad)

