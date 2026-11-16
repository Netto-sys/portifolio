# 🚀 Portfólio Profissional - Matheus Netto

## 👤 Nome do Aluno
* **Matheus Alecsander Fukuyama Netto**

## 📄 Descrição do Portfólio
Este repositório contém o código-fonte do meu site de portfólio pessoal e acadêmico. O projeto foi desenvolvido com o objetivo de servir como uma vitrine digital para mostrar minha trajetória, destacar minhas competências técnicas e apresentar os projetos que desenvolvi na área de desenvolvimento de sistemas.

## 🛠️ Tecnologias Utilizadas
* **HTML5:** Estruturação semântica das páginas e seções.
* **CSS3:** Estilização visual, layout personalizado e responsividade.
* **Bootstrap 5.3.3:** Framework CSS utilizado para agilizar o design responsivo, barra de navegação, cards e componentes visuais.
* **Devicon:** Biblioteca de ícones oficiais para representação visual das tecnologias.
* **Biblioteca AOS (Animate On Scroll):** Para renderização de animações dinâmicas e fluidas durante a rolagem da página.
* **Git & GitHub:** Versionamento de código e hospedagem/publicação do projeto.

## 🔗 Link do Site Publicado
* Acesse o projeto online em: https://netto-sys.github.io/portifolio

## ⚙️ Explicação do Funcionamento do Projeto
O site está estruturado em uma página única (*Single Page Application*) com rolagem suave ancorada pelas seções principais:
1. **Cabeçalho/Menu de Navegação (`Navbar`):** Fixo no topo da tela com links diretos para as seções do site, facilitando a navegação rápida do usuário.
2. **Carrossel Inicial:** Um componente dinâmico localizado logo no início da página.
3. **Seção Perfil:** Apresenta uma foto de, resumo biográfico profissional, cards informativos com dados de localização, formação técnica (Desenvolvimento de Sistemas e Mecatrônica) e uma listagem detalhada das principais ferramentas e linguagens dominadas.
4. **Seção Projetos:** Um grid responsivo de cards que exibe os trabalhos realizados (como este próprio portfólio, sistemas em lógica Python e páginas responsivas), contendo imagens ilustrativas, descrições objetivas e botões de acesso.
5. **Seção Contato:** Centraliza os meios de comunicação direta (e-mail, redirecionamentos para o GitHub e LinkedIn) e dados geográficos.

## ✨ Descrição do Recurso Novo Adicionado
Como nova funcionalidade e melhoria de experiência do usuário (**UX/UI**), foi implementada uma **camada de animações e microinterações baseada na rolagem da página (Scroll Animations)**. Agora, os elementos do site (como títulos, blocos de texto, cards de projetos e a foto de perfil) não aparecem estáticos de uma só vez; eles entram em cena com efeitos visuais suaves de fade e deslocamento conforme o visitante desce a tela, além de efeitos interativos de elevação (*hover*) nos cards e botões.

## 💻 Explicação de Como Esse Recurso Foi Implementado
O recurso foi integrado combinando duas abordagens eficientes:
1. **Animações e Efeitos com CSS Puro (`style.css`):**
   * Foi ativada a rolagem suave global através da propriedade `scroll-behavior: smooth;`.
   * Foram aplicadas regras de transição (`transition`) combinadas com transformações de eixo (`transform: translateY()`, `scale()`) e sombras dinâmicas (`box-shadow`) para que os cards e a foto de perfil respondam visualmente quando o mouse passa por cima.
2. **Biblioteca AOS (Animate On Scroll):**
   * Os scripts e estilos da biblioteca externa **AOS** foram importados via CDN no cabeçalho e rodapé do `index.html`.
   * A biblioteca foi inicializada via JavaScript com a configuração de duração (`duration: 800ms`) e execução única por sessão (`once: true`).
   * Atributos HTML customizados como `data-aos="fade-right"`, `data-aos="fade-up"` e `data-aos-delay` foram distribuídos estrategicamente nas tags das seções para criar um efeito de cascata visual fluido e profissional durante o carregamento e a navegação.