# 🧩 Ultimate Maze Sandbox

> Um ambiente interativo e modular em Python para geração de labirintos, simulação de algoritmos de busca (Pathfinding) e navegação em mapas reais do mundo.

---

## 📸 Demonstração do Projeto

<p align="center">
  <img src="watermarked_img_7819767323066790482.jpg" alt="Ultimate Maze Sandbox Concept" width="800"/>
</p>

---

## 🚀 Sobre o Projeto

O **Ultimate Maze Sandbox** é um simulador leve e modular projetado para visualização de algoritmos de busca e exploração de mapas. 

O projeto conta com suporte a **visões 2D/3D**, simulação em **tempo real com múltiplos agentes ("achadores")**, e um **Modo Mapa Real** capaz de integrar ruas de cidades reais via **OpenStreetMap** sem exigir nenhuma biblioteca externa pesada.

---

## ✨ Principais Funcionalidades

### 🌐 Modo Mapa Real (OpenStreetMap)
* **Busca Global:** Digite qualquer cidade ou local do mundo (ex: *"Avenida Paulista, São Paulo"*) para carregar o mapa de ruas instantaneamente.
* **Grafo Vetorial de Ruas:** Processa cruzamentos (nós) e vias (arestas) reais.
* **Carregamento Otimizado (Lazy Loading & Cache):** Sistema assíncrono em segundo plano (Threading) para evitar travamentos na interface, com salvamento local em cache.

### 📐 Modos de Visualização
* **2D Clássico (Top-Down):** Visão superior com câmera centralizada, zoom e navegação fluida.
* **3D Isométrico / Orbital:** Rotacione o labirinto em 360°, altere a elevação (pitch) e acompanhe os agentes em 3D.
* **1ª Pessoa (Dungeon Crawler):** Caminhe célula a célula pelo labirinto com detecção de colisão e um **Minimapa 2D flutuante (HUD)** no canto da tela.

### 🧠 Algoritmos de Pathfinding & Simulação
* Algoritmos de busca como **A\*** e **Dijkstra** aplicados diretamente em grades ou grafos viários.
* Suporte a múltiplos waypoints, chaves e obstáculos dinâmicos.
* Ajuste de velocidade da simulação em tempo real.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.x
* **Interface Gráfica:** `pygame`
* **APIs de Mapas:** OpenStreetMap (Nominatim & Overpass API)
* **Bibliotecas Nativas Utilizadas:** `urllib.request`, `json`, `threading`, `math`

> ⚠️ **Zero Dependências Pesadas:** Não é necessário instalar bibliotecas como `requests`, `networkx` ou `osmnx`. Tudo é processado com módulos nativos do Python!

---

## 📦 Como Executar

### Pré-requisitos
Apenas o **Python 3.8+** e o **Pygame** instalados.

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/ultimate-maze-sandbox.git](https://github.com/seu-usuario/ultimate-maze-sandbox.git)
   cd ultimate-maze-sandbox
