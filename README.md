# 🍷 Vinharia Agnello

Site institucional da Vinharia Agnello, desenvolvido como projeto de checkpoint da disciplina de Front-end. O site apresenta a história, produtos, galeria e informações de contato da vinharia, com foco em HTML semântico e boas práticas de CSS.

## 🔗 Acesse o Site

[https://lucx-yan.github.io/Vinharia-Agnello/](https://lucx-yan.github.io/Vinharia-Agnello/)

## 📋 Sobre o Projeto

O projeto Vinharia Agnello é um site institucional simples que apresenta uma vinharia fictícia, desenvolvido para demonstrar conhecimentos em HTML5 semântico e CSS3. O site possui navegação intuitiva e design responsivo, oferecendo uma experiência completa ao visitante.

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estruturação semântica (header, main, section, nav, footer)
- **CSS3** - Estilização em arquivo único (src/css/style.css)
- **GitHub Pages** - Hospedagem e deploy

## 📁 Estrutura do Projeto

```
Vinharia-Agnello/
│
├── index.html                 # Página inicial
├── README.md                  # Documentação do projeto
├── src/
│   ├── assets/
│   │   └── imgs/             # Imagens do site
│   ├── css/
│   │   ├── style.css         # Arquivo de estilos principais
│   │   └── efeitos.css       # Efeitos visuais e animações
│   └── pages/
│       ├── contato.html      # Página de contato
│       ├── galeria.html      # Galeria de fotos e vídeo
│       ├── historia.html     # História da vinharia
│       └── produtos.html     # Catálogo de vinhos
```

## 📄 Páginas

**Página Inicial (index.html)**  
A página inicial dá as boas-vindas ao visitante com um resumo sobre a vinharia e disponibiliza navegação clara para as demais seções do site, oferecendo uma primeira impressão acolhedora e profissional.

**História (historia.html)**  
Conta a trajetória da Vinharia Agnello, destacando seus diferenciais e valores que a tornam única no mercado. Esta página apresenta a essência e os princípios que guiam a produção dos vinhos da casa.

**Produtos (produtos.html)**  
O visitante encontra o catálogo completo organizado em uma tabela com diferentes categorias de vinhos acompanhadas de imagens ilustrativas, facilitando a visualização e escolha dos produtos disponíveis.

**Galeria (galeria.html)**  
Oferece uma experiência visual com fotos dos ambientes internos da vinharia e um vídeo de tour virtual incorporado do YouTube, permitindo que o visitante conheça as instalações de forma imersiva.

**Contato (contato.html)**  
Disponibiliza um formulário para o visitante enviar mensagens com campos de nome, e-mail e mensagem, além de um mapa integrado do Google Maps indicando a localização da vinharia para facilitar o acesso presencial.

## ✨ Efeitos Visuais 

### 🎯 Pseudo-classes Implementadas

**1. `:hover` - Interação nos links de navegação**
- Aplicado em: Links do menu de navegação (todas as páginas)
- Efeito: Cor muda para vinho escuro, fundo dourado semi-transparente, bordas arredondadas
- Melhora a experiência do usuário indicando claramente elementos clicáveis

**2. `:focus` - Destaque em campos de formulário**
- Aplicado em: Inputs e textarea do formulário de contato
- Efeito: Borda vermelha espessa (5px), sombra suave, fundo levemente amarelado, leve aumento de escala
- Melhora a acessibilidade mostrando qual campo está ativo

**3. `:first-child` - Destaque no primeiro item**
- Aplicado em: Primeiro link de cada menu de navegação
- Efeito: Texto em negrito, cor vinho escuro, borda esquerda dourada (4px)
- Cria hierarquia visual na navegação

**4. `:nth-child(odd/even)` - Efeito zebrado na tabela**
- Aplicado em: Linhas da tabela de produtos
- Efeito: Linhas ímpares com fundo dourado claro, linhas pares com fundo vinho suave
- Facilita a leitura de tabelas extensas

**5. `:hover` nas imagens**
- Aplicado em: Imagens dos produtos (`.vinho`) e da galeria (`.gal`)
- Efeito: Aumento de tamanho com transição suave de 0.5s
- Permite visualização detalhada das imagens

### 🎨 Pseudo-elementos Implementados

**1. `::selection` - Seleção de texto personalizada**
- Aplicado em: Todos os parágrafos do site
- Efeito: Fundo vinho escuro, texto dourado
- Mantém identidade visual da marca mesmo ao selecionar texto

**2. `::marker` - Marcadores de lista personalizados**
- Aplicado em: Todas as listas do site
- Efeito: Marcadores dourados com tamanho aumentado (22px)
- Adiciona consistência visual aos elementos de lista

**3. `::after` - Linha decorativa em títulos**
- Aplicado em: Títulos h2 e h3 dentro do main
- Efeito: Linha decorativa com gradiente (vinho → dourado), animação de expansão ao carregar
- Adiciona sofisticação visual aos títulos de seção

### 💫 Animações com @keyframes

**1. `aparecer` - Entrada suave do título**
- Aplicada em: h1 do header
- Duração: 1.5 segundos
- Efeito: Título aparece com fade-in e movimento vertical suave
- Cria impacto visual ao carregar a página

**2. `pulsar` - Pulsação nos botões**
- Aplicada em: Botões ao passar o mouse
- Duração: 1 segundo (loop infinito)
- Efeito: Botão aumenta 5% e retorna ao tamanho normal
- Chama atenção para ações importantes

**3. `expandLine` - Expansão da linha decorativa**
- Aplicada em: Pseudo-elemento `::after` dos títulos h2 e h3
- Duração: 1.2 segundos
- Efeito: Linha cresce da esquerda para direita
- Adiciona dinamismo ao carregamento da página

### 🎢 Transformações CSS

**1. `scale()` - Zoom nas imagens de produtos**
- Aplicado em: Imagens com classe `.vinho`
- Valor: 1.1 (aumento de 10%)
- Transição: 0.5s ease
- Permite visualização detalhada dos produtos

**2. `scale()` - Zoom nas imagens da galeria**
- Aplicado em: Imagens com classe `.gal`
- Valor: 1.15 (aumento de 15%)
- Transição: 0.5s ease
- Efeito mais intenso para fotos da galeria

**3. `translateX()` - Movimento nos itens do menu**
- Aplicado em: Itens da lista de navegação
- Valor: 10px para a direita
- Transição: 0.3s ease
- Feedback visual ao interagir com o menu

**4. `scale()` - Aumento nos botões**
- Aplicado em: Todos os botões ao hover
- Valor: 1.05 (aumento de 5%)
- Transição: 0.3s ease
- Indica que o elemento é clicável

### 🔄 Transições Aplicadas

Todas as transformações e mudanças de estado utilizam transições suaves para melhorar a experiência do usuário:
- **Links**: Transição de cor e fundo
- **Imagens**: Transição de transformação (scale)
- **Botões**: Transição de transformação e animação
- **Campos de formulário**: Transição de borda, sombra e escala
- **Tabela**: Transição de cor de fundo
- **Menu**: Transição de posição (translateX)

## 👥 Equipe de Desenvolvimento

- **João Victor (RM: 566640)**
- **Gabriel Amparo (RM: 568274)**
- **Gustavo Macedo (RM: 567594)**
- **Gustavo Hiruo (RM: 567625)**
- **Yan Lucas (RM: 567046)**

## 📝 Licença

Este projeto foi desenvolvido para fins educacionais como parte do checkpoint de Front-end.

---

⭐ Desenvolvido com dedicação pela equipe Vinharia Agnello