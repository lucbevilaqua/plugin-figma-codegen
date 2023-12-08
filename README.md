# Figma Classify

O Figma Classify é um plugin projetado para melhorar a eficiência e a organização dos designers e desenvolvedores no Figma. Utilizando a interface "Generate Code" nativo do figma no modo DEV, o plugin permite que os usuários visualizem e copiem rapidamente nomes de classes CSS e tags HTML geradas automaticamente com base nas instâncias selecionadas. 

OBS: esse plugin gera classes CSS e codigo de tag HTML apenas para elementos variantes de componentes (Instancias) e para os Frame que utilizam auto-layout o plugin gera uma class "spacing-p-${x}" (onde X é uma variavel relacionando px com rem).

## Estrutura de Pastas

- **main.ts**: Aqui é onde nossa aplicação conversa com a API do figma.
- **manifest**: Arquivo que importamos para o figma com nossa configuração.

## Instalação
Antes de iniciar o projeto, certifique-se de ter o [Node.js](https://nodejs.org/) ou [yarn](https://yarnpkg.com/) e o [Figma Desktop](https://www.figma.com/downloads/) instalados no seu sistema.

Para instalar as dependências do projeto, execute o seguinte comando no terminal na raiz do projeto:

```bash
  npm install
```
    
## Como rodar o projeto

Voce pode consultar mais detalhadamente na documentação oficial [plugin-quickstart-guide](https://www.figma.com/plugin-docs/plugin-quickstart-guide/)

**Siga os passos abaixo para rodar o plugin no figma**:
1. Rode o seguinte comando em seu terminal do projeto```bash npm run watch ```
2. No seu projeto do figma clique em plugins -> manage plugins...
2. Na sessão de plugins altere o seletor para mostrar os plugins do modo development
3. Clique no botao "Novo" ou "+" para adicionar um novo plugin e em seguida selecione a opcao "import plugin from manifest..."
4. Navegue até a pasta do projeto e selecione o arquivo manifest
5. Pronto, agora só ativar o modo DEV do figma e olhar no sidebar direito até a sessão "Code" (imagem abaixo).

<p align="center">
  <img src="https://github.com/lucbevilaqua/plugin-figma-classify/assets/77061281/e62a489d-c636-4f57-a08e-5133310a328d" />
</p>

## Licença

[MIT](https://choosealicense.com/licenses/mit/)