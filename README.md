# 📄 README.md - Invasores Zumbis

```markdown
# 🧟 Invasores Zumbis

> Um jogo de sobrevivência 2D desenvolvido inteiramente com **HTML5**, **CSS3** e **JavaScript puro** — sem frameworks, sem bibliotecas externas, sem dependências.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge)]()
[![Licença](https://img.shields.io/badge/Licença-MIT-blue?style=for-the-badge)](#-licença)

---

## 📖 Sobre o Jogo

**Invasores Zumbis** é um jogo de ação arcade onde o jogador assume o papel de um sobrevivente isolado no centro da tela, cercado por hordas de zumbis que surgem continuamente das bordas. Com apenas uma arma e reflexos rápidos, o objetivo é eliminar o maior número possível de mortos-vivos antes que eles alcancem sua posição.

A dificuldade aumenta progressivamente conforme o tempo passa: os zumbis surgem com mais frequência e se movem cada vez mais rápido, testando os limites do jogador.

---

## ✨ Características

- 🎮 **Gameplay simples e viciante** — fácil de aprender, difícil de dominar
- 🧟 **Spawn inteligente** — zumbis aparecem fora da tela e caminham em direção ao centro
- 🎯 **Mira precisa** — atire na direção exata do cursor com o botão direito
- 💥 **Efeitos visuais** — partículas de explosão, brilho nos tiros e flash de morte
- 📈 **Dificuldade crescente** — desafio progressivo baseado no tempo de sobrevivência
- ⏸️ **Sistema de pausa** — pause a qualquer momento com a tecla `P`
- 📱 **Responsivo** — adapta-se a qualquer tamanho de tela
- 🖥️ **Alta resolução** — suporte a telas Retina/HiDPI
- 🚀 **Leve e rápido** — arquivo único, sem dependências, carrega instantaneamente

---

## 🎮 Como Jogar

### Controles

| Ação | Comando |
|------|---------|
| 🖱️ Atirar | **Botão direito do mouse** (na direção do cursor) |
| ⏸️ Pausar / Continuar | Tecla `P` |
| 🔄 Iniciar / Reiniciar | Tecla `F1` ou botão na tela |

### Objetivo

- Elimine os zumbis antes que eles cheguem ao centro da tela.
- Cada zumbi eliminado vale **1 ponto**.
- O jogo termina quando um zumbi alcança o jogador.
- Tente bater seu recorde de pontuação!

---

## 🚀 Como Executar

### Opção 1 — Abrir diretamente no navegador (recomendado)

1. Baixe o arquivo `invasores-zumbis.html` deste repositório.
2. Dê um duplo clique no arquivo ou abra-o com seu navegador preferido.
3. Pressione `F1` ou clique em **Jogar** para começar!

### Opção 2 — Servir localmente (para desenvolvimento)

Se preferir servir via HTTP (recomendado para evitar restrições de CORS em alguns navegadores):

```bash
# Usando Python 3
python -m http.server 8000

# Usando Node.js (npx)
npx serve .
```

Depois acesse: `http://localhost:8000/invasores-zumbis.html`
```
### Opção 3 — Hospedar online

O jogo é um arquivo HTML estático, então pode ser hospedado em qualquer serviço:
- [GitHub Pages](https://pages.github.com/)
- [Netlify](https://www.netlify.com/)
- [Vercel](https://vercel.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)
```
---
```
## 🛠️ Tecnologias Utilizadas

- **HTML5** — Estrutura do documento e elemento `<canvas>`
- **CSS3** — Interface, layout responsivo, variáveis CSS, animações
- **JavaScript (ES6+)** — Lógica do jogo, classes, loop de renderização com `requestAnimationFrame`
- **Canvas 2D API** — Renderização de sprites, partículas, efeitos visuais

> ⚠️ **Nenhum framework ou biblioteca externa foi utilizado.** Todo o código foi escrito do zero.

---
```
## 📂 Estrutura do Projeto

```
invasores-zumbis/
├── README.md                  # Este arquivo
└── invasores-zumbis.html      # Jogo completo (HTML + CSS + JS em um único arquivo)
```

O projeto foi pensado para ser **o mais simples possível**: um único arquivo HTML autocontido, facilitando distribuição, hospedagem e compartilhamento.

---

## 🧠 Processo de Desenvolvimento

O jogo foi desenvolvido em **5 etapas iterativas**, cada uma validada antes de avançar para a próxima:

| Etapa | Descrição | Status |
|-------|-----------|--------|
| 1 | Validação do plano de desenvolvimento | ✅ Concluída |
| 2 | Mecânica de mira e disparo (classe `Tiro`) | ✅ Concluída |
| 3 | Spawning e inteligência dos zumbis (classe `Zumbi`) | ✅ Concluída |
| 4 | Colisões, pontuação e regras de jogo | ✅ Concluída |
| 5 | Polimento visual e empacotamento final | ✅ Concluída |

### Principais conceitos aplicados:

- **Máquina de estados** (`MENU`, `PLAYING`, `GAME_OVER`)
- **Game Loop** com `requestAnimationFrame` e delta time (`dt`)
- **Programação Orientada a Objetos** (classes `Tiro`, `Zumbi`, `Particula`)
- **Trigonometria** para cálculos de ângulo e direção (`Math.atan2`)
- **Detecção de colisão** por distância entre círculos
- **Sistema de partículas** para efeitos visuais
- **Gerenciamento de memória** (remoção de objetos inativos)

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Se você tem ideias para melhorar o jogo:

1. Faça um **Fork** do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um **Pull Request**

### 💡 Ideias para futuras melhorias:

- [ ] Sistema de power-ups (tiro múltiplo, escudo, bomba)
- [ ] Diferentes tipos de zumbis (rápido, tanque, voador)
- [ ] Efeitos sonoros e música de fundo
- [ ] Sistema de high score salvo no `localStorage`
- [ ] Modos de jogo (sobrevivência, onda, chefe)
- [ ] Suporte a dispositivos móveis (touch)
- [ ] Leaderboard online

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License** — veja o arquivo [LICENSE](LICENSE) para detalhes.

```
MIT License

Copyright (c) 2026 Invasores Zumbis

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
