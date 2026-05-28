# 🧠 Heurísticas e Modelagem Multiobjetivo

<div align="center">

![Status](https://img.shields.io/badge/status-em_andamento-yellow?style=for-the-badge)
![Python](https://img.shields.io/badge/python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/jupyter-notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Licença](https://img.shields.io/badge/licença-acadêmica-gray?style=for-the-badge)

**INF0415 — Universidade Federal de Goiás**
Bacharelado em Inteligência Artificial · 5º Período · 2026/1

</div>

---

## 📖 Sobre

Repositório de atividades práticas (TLs) da disciplina **INF0415 — Heurísticas e Modelagem Multiobjetivo**. Os notebooks cobrem desde buscas clássicas em grafos até otimização multiobjetivo, utilizando problemas consagrados como o **8-Puzzle**, **TSP** e **funções benchmark** (Rastrigin).

## 👥 Autores

| Nome | Matrícula |
|------|-----------|
| Wagner Victor Alves de Menezes | 202403929 |
| Victor Gabriel Ribeiro Jácome | 202403926 |
| Raphael Alves de Lima Soares | 202403922 |

> Atividades pontuais contam também com a participação de Igor Dias e Lucas Ozório.

---

## 🗂️ Estrutura do Repositório

```text
heuristicas/
├── busca-sistematica/
│   ├── semana2_agentes_busca.ipynb
│   ├── semana3_busca_informada.ipynb
│   └── semana4_busca_adversaria.ipynb
├── busca-local/
│   ├── semana5_busca_local.ipynb
│   └── semana6_busca_tabu.ipynb
├── metaheurísticas-populacionais/
│   ├── semana7_ag_tsp.ipynb
│   ├── semana8_pso_aco.ipynb
│   ├── semana9_memetico.ipynb
│   └── Sem10_MOO.ipynb
├── requirements.txt
└── README.md
```

---

## 📚 Conteúdo das Atividades

### Módulo 1 — Busca Sistemática

| Semana | Notebook | Tema | Descrição |
|:------:|----------|------|-----------|
| 2 | `semana2_agentes_busca.ipynb` | Agentes e Busca Não-Informada | BFS e DFS aplicados ao **8-Puzzle**; comparação de completude, otimalidade e custo computacional |
| 3 | `semana3_busca_informada.ipynb` | Busca Informada | Heurísticas (Manhattan, Hamming), **A\*** e **IDA\*** no 8-Puzzle; comparação com BFS |
| 4 | `semana4_busca_adversaria.ipynb` | Busca Adversária | **Minimax** e **poda Alfa-Beta** para Jogo da Velha e Connect Four; torneio entre agentes |

### Módulo 2 — Busca Local

| Semana | Notebook | Tema | Descrição |
|:------:|----------|------|-----------|
| 5 | `semana5_busca_local.ipynb` | Hill Climbing e Simulated Annealing | Otimização da **função Rastrigin** e do **TSP** com métodos de vizinhança |
| 6 | `semana6_busca_tabu.ipynb` | Busca Tabu | Implementação de Busca Tabu no TSP; comparativo com HC e SA |

### Módulo 3 — Metaheurísticas Populacionais

| Semana | Notebook | Tema | Descrição |
|:------:|----------|------|-----------|
| 7 | `semana7_ag_tsp.ipynb` | Algoritmos Genéticos | GA com `deap` para o TSP: seleção, crossover (OX/PMX), mutação e elitismo |
| 8 | `semana8_pso_aco.ipynb` | Inteligência de Enxame | **PSO** na Rastrigin (n=10) e **ACO** no TSP; implementação from-scratch |
| 9 | `semana9_memetico.ipynb` | Algoritmos Meméticos | GA + **2-opt** (Lamarckiano) e Warm-Start para TSP; competição Algorithm Discovery |
| 10 | `Sem10_MOO.ipynb` | Otimização Multiobjetivo | **NSGA-II** e **SPEA-II** com `pymoo` para TSP biobjetivo (distância × pedágio) |

---

## 🔗 Progressão Temática

```
Busca Não-Informada (BFS/DFS)
  └──▶ Busca Informada (A*/IDA*)
        └──▶ Busca Adversária (Minimax/α-β)
              └──▶ Busca Local (HC / SA / Tabu)
                    └──▶ Metaheurísticas Populacionais (GA / PSO / ACO)
                          └──▶ Algoritmos Meméticos (GA + 2-opt)
                                └──▶ Otimização Multiobjetivo (NSGA-II / SPEA-II)
```

---

## ▶️ Como Executar

### Pré-requisitos

- Python 3.x
- `pip` ou `conda`

### Instalação

```bash
# Clone o repositório
git clone https://github.com/<seu-usuario>/heuristicas.git
cd heuristicas

# Crie e ative um ambiente virtual
python -m venv .venv
source .venv/bin/activate   # Linux/macOS
# .venv\Scripts\activate    # Windows

# Instale as dependências
pip install -r requirements.txt
```

### Execução

Abra os notebooks com **Jupyter**, **VS Code** ou qualquer ferramenta compatível com `.ipynb`:

```bash
jupyter notebook
```

> **Nota:** Alguns notebooks requerem bibliotecas adicionais (`deap`, `pymoo`) que são instaladas automaticamente nas primeiras células de cada notebook.

---

## 🛠️ Dependências

| Biblioteca | Uso |
|------------|-----|
| `numpy` | Operações numéricas e vetoriais |
| `pandas` | Manipulação de dados tabulares |
| `matplotlib` | Visualizações e gráficos |
| `deap` | Framework para Algoritmos Genéticos (Semana 7) |
| `pymoo` | Otimização Multiobjetivo (Semana 10) |

---

## 📄 Licença

Material acadêmico produzido para fins educacionais na disciplina INF0415 — UFG.
