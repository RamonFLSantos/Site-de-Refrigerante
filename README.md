# Amostra de Refrigerantes — HTML, CSS e JavaScript

Projeto pessoal desenvolvido para treinar animações no Frontend utilizando **HTML, CSS e JavaScript puros**.  
A aplicação apresenta uma **galeria animada de refrigerantes**, onde o usuário pode navegar entre diferentes sabores por meio de um slider simples e fluido.

---

## Tecnologias utilizadas

- **HTML5**
- **CSS3**
- **JavaScript Vanilla**
- **Git + Git Flow**

---

## Funcionalidades

- Slider animado com transição suave entre sabores.
- Destaque para cor, imagem e título de cada refrigerante.
- Navegação por botões (`prev` e `next`).
- Animação de entrada dos elementos (frutas, título e lata).

---

## Git Flow aplicado

O projeto segue a estrutura tradicional do **Git Flow**, mantendo o desenvolvimento organizado e separado por níveis de estabilidade:

- **main** → versão estável e pronta para produção  
- **dev** → ambiente de desenvolvimento onde novas funcionalidades são integradas  
- **feat/*** → branches de feature criadas a partir de `dev` para implementar melhorias específicas

### Fluxo utilizado

1. Criar uma nova branch de feature a partir de `dev`:
2. Desenvolver normalmente e fazer commits seguindo boas práticas (`feat:`, `fix:`, etc.).
3. Ao terminar a feature, fazer merge para `dev`:
   git checkout dev
  git merge feat/nome-da-feature
4. Quando a versão estiver estável e testada em `dev`, fazer merge para `main`:
   
### Estrutura atual das branches

- `main` (default)  
- `dev` (desenvolvimento contínuo)  
- `feat/index-development` (feature relacionada ao desenvolvimento da página inicial)

Essa abordagem garante:
- Organização do código  
- Fluxo claro entre desenvolvimento e produção  
- Histórico limpo  
- Facilidade de expansão do projeto

---

## Como funciona o slider

- Cada refrigerante é representado por um `.item`
- Apenas o item com a classe `.active` fica visível
- O JavaScript remove essa classe do item atual e adiciona ao próximo/anterior
- As animações de fade/entrada são controladas por:

```css
@keyframes toActive {
  from {
    top: 100%;
    opacity: 0;
  }
}
```

---

## Objetivo do Projeto

Este projeto foi criado com o objetivo de treinar animações e interações visuais no Frontend utilizando HTML, CSS e JavaScript.  
A proposta envolve construir um slider animado de refrigerantes, explorando:

- Estruturação de layout em HTML
- Animações e transições suaves com CSS
- Manipulação do DOM com JavaScript puro
- Organização e versionamento seguindo Git Flow

O foco principal é desenvolver habilidades práticas de animação, responsividade e organização do código.
