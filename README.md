- 👋 Hi, I’m @personalboat
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
personalboat/personalboat is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

# Cinepédia-v2
Aplicação web no formato SPA, feita com React alimentada com a API do TMDB (The Movie Data Base). A aplicação possui recomendações de filmes/séries e uma busca por algum item específico.
[ Projeto Online ] ( https://cinepedia-v2.vercel.app )
# Pré-requisitos
Antes de executar este projeto, verifique se você atende aos seguintes requisitos:
1. Node.js (versão 18.16.0 ou superior)
2. Visual Studio Code (ou qualquer outro editor de sua preferência)
Certifique-se de ter o Node.js instalado em seu sistema e definido no PATH. Você pode verificar se o Node.js está instalado digitando o seguinte comando no terminal:
```
nó --versão
```
Além disso, é recomendado utilizar o Visual Studio Code como editor de código, mas você pode optar por qualquer outro editor de sua preferência.
# Para utilizar o Projeto
Siga as etapas abaixo para configurar e executar o projeto:
1. Adicione sua chave no TMDB em src/services/api.js.
2. No prompt, navegue até a pasta raiz do projeto.
3.Instale as dependências necessárias executando o comando:
```
instalação de fios
```
ou
```
instalação npm
```
4. Rode o projeto utilizando o comando:
```
início do fio
```
ou
```
npm início
```
**Certifique-se de substituir sua-chave pelo valor correto da sua chave no arquivo `src/services/api.js`.**
# Créditos
1 . Ícone da aplicação retirada do site Flaticon: < a  href = " https://www.flaticon.com/free-icons/cinema "  title = " cinema icons " >Ícones de cinema criados por Freepik - Flaticon</ a >
2 . Fundos SVG retirados do site HeroPatterns: [ Hero Patterns ] ( https://heropatterns.com )
# Inspiração
A idéia veio do projeto AluraFlix, o último challenge do Projeto Oracle ONE da formação front-end.
A base era um site com links fixos de vídeos do YouTube baseados em algum tema.
Resolvi adaptar e fazer um site com informações de filmes e séries, alimentado por uma API.
# Funcionalidades
1. ## Carrosséis de Recomendação
    1. Na página inicial, há um carrossel com os filmes mais buscados e com as melhores notas, e também existe uma página dedicada a dois carrosséis, de novidades e futuros lançamentos.
        1. Feito com `react-alice-carousel`.
        2. O carrossel com os filmes mais buscados está disponível apenas para computador, devido as limitações de tamanho da tela. Mas página a dedicada a dois carrosséis, de novidades e futuros lançamentos permanece para a versão mobile.
    3. O carrossel gira automaticamente a cada 2 segundos, ele para de girar colocando o cursor em cima do carrossel, permitindo arrastar ou clicar nos botões para navegar entre os itens.
    4. Ao clicar no pôster, uma janela flutuante é exibida com mais informações.
        1. Para fechar a janela flutuante, basta clicar no botão fechar, pressionar a tecla ESC ou clicar fora da janela.
    5. Cada item trás o tipo de mídia (filme ou série), poster, título, nota e data de lançamento.
        1. A nota possui um css que varia de acordo com a nota, sendo preenchido com um radial grandient e varias especificações via JS para refletir melhor a nota visualmente.
2. ## Pesquisa de Filmes/Séries
     1. É possível pesquisar por um item específico (filme ou série) com 3 campos: uma palavra chave que faz parte do nome do item (obrigatório), ano de lançamento (opcional - não é o ano mínimo, mas o ano exato do lançamento), nota mínima (opcional).
     2. Ele retorna um carrossel semelhante ao carrossel de recomendações, a única diferença é que ele não gira automaticamente para o usuário poder analisar melhor os resultados, a navegação é feita arrastando ou clicando nos botões para navegar entre os itens.
3. ## Janela flutuante com detalhes dos itens
     1. A janela flutuante trás informações como: nome da mídia, tipo de mídia, gênero da mídia, ano de lançamento, sinopse (se disponível), trailers (se disponível), provedores para assistir (se disponível) - ex: amazon, netflix, etc.
         1. Janela flutuante feita com `react-modal-dialog` e devido as restrições dos frames com link por variáveis, player de vídeo feito com `react-player`.
         2. Para fechar a janela flutuante, basta clicar no botão fechar, pressionar a tecla ESC ou clicar fora da janela.
         3. Os provedores para assistir estão separados por streaming, aluguel e compra.
         3. Os provedores para assistir estão separados por streaming, aluguel e compra. Eles também estão filtrados para mostrarem somente opções que tenham conteúdo dublado ou legendado em pt-BR.
4. ## Variação de Temas - Escuro (padrão) e Claro
     1. Botão de switch de temas, que altera a imagem de background, a cor do background, a cor das sombras, a cor das fontes, a cor das bordas, etc.
         1. Feito com ThemeProvider do `styled-components`.
         2. Utilizado um hook personalizado para switch dos temas e outros componentes que precisam de controles true/false.
5. ## Responsivo
     1. Todos os itens foram trabalhados de forma responsiva, se adaptando a desktops e dispositivos móveis.
         1. Dentro do GlobalStyles, foram configuradas duas classes globais `apenas-desktop` e `apenas-mobile`, ao colocar essa classe em um item ele irá ser um item que renderiza somente em um determinado tipo de resolução.
# Imagens do Projeto
## Área de Trabalho
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/8f6bc0e9-fa10-46c3-a502-8d9b1c449e16 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/5ee0a5a0-59c1-45e1-b994-6d047d53ce0a )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/c282854a-d1f5-447f-8306-81ea81de5dcb )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/7f340fad-7802-4a57-b940-f8a89e8bf5ea )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/454529c8-14c1-418b-b4ed-0575510a90ae )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/e7e60db8-d74c-4a8b-b7d4-4c1a7f45da73 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/9c8fd6a9-4809-4b62-97c1-ca06a36c9338 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/7531ea54-84b7-4f14-9aaf-70c836013736 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/7f9735e7-521e-4c59-b90d-f68a15a55e7f )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/dda9e7a3-7bbc-40d3-be3c-65033769e633 )
## Móvel
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/25f167d4-92c8-4a6f-b1fa-5009e33c6c70 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/2c4b85bc-c2c5-43d1-bede-c0d5f59e3080 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/3fa826cc-bf24-481a-a82d-9089296bd190 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/7cc6e3a8-b7f3-4407-bc12-abc2b041bdb5 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/91fe2018-11f3-4e82-ba60-424ae47fd9da )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/fcb16639-f38c-4202-8a20-2a73b06b8048 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/e59bd067-0e71-4746-a2bc-4332da7f32b7 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/e01c35ed-5896-4eec-b26b-265c6f51fb3f )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/32b2b9dc-8e80-456e-9c02-c88eacaa4643 )
![ imagem ] ( https://github.com/leticiapalaro/cinepedia-react-tmdb/assets/109923860/2a86ae25-9c7c-4aca-9098-f45599e4868f )
# Sobre a Dev
Olá! Sou Letícia Palaro, uma mulher entusiasmada e determinada, formada em Análise e Desenvolvimento de Sistemas e atualmente cursando uma pós-graduação em Gestão de Projetos.
Desde a minha infância, fui cativada pela tecnologia. Tudo começou com o incrível universo dos jogos, onde embarquei em emocionantes aventuras com o meu querido Nintendo64. À medida que o tempo passava, acompanhei a evolução tecnológica, migrando para os jogos de computador e experimentando novas possibilidades.
Sou movida pela paixão de aprender constantemente, e essa mentalidade me impulsiona a me concentrar ao máximo nas minhas atividades.
Com determinação e entusiasmo, estou pronta para enfrentar os desafios futuros e contribuir para um mundo impulsionado pela tecnologia.
# Contato
< div  align = " centro " >
  < img  altura = " 200vh "  fonte = " https://github.com/leticiapalaro/leticiapalaro/blob/main/ok.gif?raw=true " >< br > < a  href = " https://www.linkedin.com/in/leticiapalaro/ "  alvo = " _blank " >< img  altura = " 25vh "  fonte = " https://github.com/leticiapalaro/leticiapalaro/blob/main/linkedin.png?raw=true "  alvo = " _blank " ></ a >
  < a  href = " mailto:leticiapalaro@live.com " >< img  height = " 25vh "  src = " https://github.com/leticiapalaro/leticiapalaro/blob/main/contato.png?raw=true "  target = " _blank " ></ a >< br >
</div>
