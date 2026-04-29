# 🎨 Color Matcher: O Quão Bom é o Seu Olho? 👀

Um minigame simples e interativo que testa a sua percepção visual. O sistema gera uma cor RGB aleatória e o seu objetivo é tentar replicá-la usando qualquer ferramenta de Color Picker externa, colar o print no site e descobrir a sua taxa de precisão!

## 🚀 Como Jogar

1. Abra a aplicação no navegador. Uma **Cor Alvo** será gerada aleatoriamente.
2. Vá em qualquer site ou ferramenta de **Color Picker** (como o do próprio Google).
3. Tente escolher a cor que mais se aproxima da cor alvo.
4. Tire um **print/captura de tela** da cor que você escolheu.
5. Volte para a página do jogo, clique em qualquer lugar e pressione `Ctrl + V`.
6. Clique no botão **"Revelar Precisão!"** para descobrir a diferença real entre os códigos RGB e a sua porcentagem de acerto.

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído puramente com tecnologias front-end nativas, sem dependências externas:

* **HTML5 & CSS3:** Estrutura e estilização da interface.
* **Vanilla JavaScript:** Lógica principal do jogo.
* **Clipboard API:** Para interceptar e ler os dados da imagem direto da área de transferência do usuário (`Ctrl+V`).
* **Canvas API:** Utilizado nos bastidores para renderizar a imagem colada, extrair a matriz de pixels RGBA e calcular a cor média com base em todos os pixels da amostra.
* **Matemática (Distância Euclidiana):** Utilizada no espaço tridimensional (R, G, B) para calcular a distância exata entre a cor alvo e a cor do usuário, convertendo o resultado em uma porcentagem de precisão de 0% a 100%.

## 💻 Como rodar o projeto localmente

Como o projeto não requer um back-end, basta clonar o repositório e abrir o arquivo no navegador:

```bash
git clone https://github.com/Miguel-Edson/Color_Game.git