<p align="center">
  <strong>🇺🇸 <a href="#-english-version"> English</a> | 🇧🇷 <a href="#-versao-em-portugues">Português</a></strong>
</p>

---

<a id="-english-version"></a>

# Facial Recognition and Logistics Optimization for Distribution Centers

##  About the Project

Official repository of the project developed for the **Melhores Compras Challenge** as part of
**FIAP's Phase 6**. The solution combines two Artificial Intelligence approaches applied to the
context of **automated pickup centers**:

1. **Computer Vision (Facial Recognition)** - customer identification for automated release of
   parcels at pickup centers.
2. **Unsupervised Machine Learning (Clustering)** - logistics optimization to strategically
   define the location of new distribution centers.

---

##  Goals

- Automate customer authentication at pickup points through facial recognition.
- Reduce delivery failures by positioning distribution centers intelligently.
- Demonstrate, in practice, the application of AI techniques to a real retail and logistics scenario.

---

##  Repository Structure

```
facial-recognition-distribution-centers/
├── 01_Reconhecimento_Facial.ipynb                  # Facial detection and recognition (OpenCV)
├── 02_Clusterizacao_Logistica_KMeans.ipynb         # Logistics optimization (K-Means)
├── Fiap On - Fase 6 - Geolocalização Dataset - Asset.csv   # Geolocation dataset
├── imagens_faces/                                  # Image base (5 people)
│   ├── pessoa_1/ ... pessoa_5/                      # 6 photos per person
├── Relatorio_Melhores_Compras_Os_Mosqueteiros.pdf  # Technical project report
└── README.md
```

---

##  Part 1 - Facial Recognition

Notebook: **`01_Reconhecimento_Facial.ipynb`**

Uses OpenCV's **Haar Cascade** classifier for facial detection. For each person in the base, the
first photos are used as **reference (training)** and the remaining ones as **validation (testing)**,
simulating the customer authentication flow at the pickup center.

**Techniques and libraries:**

- `OpenCV (cv2)` - facial detection with Haar Cascade
- `NumPy` - image array manipulation
- `Matplotlib` - results visualization

---

##  Part 2 - Logistics Optimization (K-Means)

Notebook: **`02_Clusterizacao_Logistica_KMeans.ipynb`**

Applies the **K-Means** algorithm to a geolocation dataset of delivery failures to identify
**5 clusters**. The resulting centroids indicate the ideal location for the new **pickup centers
(hubs)**, reducing the average delivery distance.

**Techniques and libraries:**

- `pandas` - dataset loading and processing
- `scikit-learn (KMeans)` - unsupervised clustering
- `Matplotlib` - visualization of clusters and centroids

---

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<user>/facial-recognition-distribution-centers.git
   cd facial-recognition-distribution-centers
   ```

2. Install the dependencies:
   ```bash
   pip install opencv-python numpy pandas scikit-learn matplotlib jupyter
   ```

3. Open the notebooks:
   ```bash
   jupyter notebook
   ```

4. Run the cells of **`01_Reconhecimento_Facial.ipynb`** and
   **`02_Clusterizacao_Logistica_KMeans.ipynb`** in the presented order.

---

## Technologies Used

| Category               | Tools                                |
| ---------------------- | ------------------------------------ |
| Language               | Python 3.x                           |
| Computer Vision        | OpenCV (Haar Cascade)                |
| Machine Learning       | scikit-learn (K-Means)               |
| Data Manipulation      | pandas, NumPy                        |
| Visualization          | Matplotlib                           |
| Environment            | Jupyter Notebook                     |

---

##  Documentation

The complete technical report of the project is available at
**`Relatorio_Melhores_Compras_Os_Mosqueteiros.pdf`**.

---

##  Team - Os Mosqueteiros

Project developed by the **Os Mosqueteiros** group for FIAP's Phase 6.

---


---

<a id="-versao-em-portugues"></a>

# Reconhecimento Facial e Otimização Logística para Centros de Distribuição

##  Sobre o Projeto

Repositório oficial do projeto desenvolvido para o **Challenge Melhores Compras** no âmbito da
**Fase 6 da FIAP**. A solução combina duas frentes de Inteligência Artificial aplicadas ao
contexto de **centros de retirada automatizados (pickup centers)**:

1. **Visão Computacional (Reconhecimento Facial)** - identificação de clientes para liberação
   automatizada de encomendas nos centros de retirada.
2. **Machine Learning Não Supervisionado (Clusterização)** - otimização logística para definição
   estratégica da localização de novos centros de distribuição.

---

##  Objetivos

- Automatizar a autenticação de clientes nos pontos de retirada por meio do rosto.
- Reduzir falhas de entrega posicionando os centros de distribuição de forma inteligente.
- Demonstrar, na prática, a aplicação de técnicas de IA em um cenário real de varejo e logística.

---

##  Estrutura do Repositório

```
facial-recognition-distribution-centers/
├── 01_Reconhecimento_Facial.ipynb                  # Detecção e reconhecimento facial (OpenCV)
├── 02_Clusterizacao_Logistica_KMeans.ipynb         # Otimização logística (K-Means)
├── Fiap On - Fase 6 - Geolocalização Dataset - Asset.csv   # Dataset de geolocalização
├── imagens_faces/                                  # Base de imagens (5 pessoas)
│   ├── pessoa_1/ ... pessoa_5/                      # 6 fotos por pessoa
├── Relatorio_Melhores_Compras_Os_Mosqueteiros.pdf  # Relatório técnico do projeto
└── README.md
```

---

## Parte 1 - Reconhecimento Facial

Notebook: **`01_Reconhecimento_Facial.ipynb`**

Utiliza o classificador **Haar Cascade** do OpenCV para detecção facial. Para cada pessoa da base,
as primeiras fotos são usadas como **referência (treino)** e as demais como **validação (teste)**,
simulando o fluxo de autenticação de um cliente no centro de retirada.

**Técnicas e bibliotecas:**

- `OpenCV (cv2)` - detecção facial com Haar Cascade
- `NumPy` - manipulação de arrays de imagem
- `Matplotlib` - visualização dos resultados

---

##  Parte 2 - Otimização Logística (K-Means)

Notebook: **`02_Clusterizacao_Logistica_KMeans.ipynb`**

Aplica o algoritmo **K-Means** sobre um dataset de geolocalização de falhas de entrega para
identificar **5 clusters**. Os centroides resultantes indicam a localização ideal dos novos
**centros de retirada (hubs)**, reduzindo a distância média das entregas.

**Técnicas e bibliotecas:**

- `pandas` - carregamento e tratamento do dataset
- `scikit-learn (KMeans)` - clusterização não supervisionada
- `Matplotlib` - visualização dos clusters e centroides

---

##  Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Biihz/facial-recognition-distribution-centers.git
   cd facial-recognition-distribution-centers
   ```

2. Instale as dependências:
   ```bash
   pip install opencv-python numpy pandas scikit-learn matplotlib jupyter
   ```

3. Abra os notebooks:
   ```bash
   jupyter notebook
   ```

4. Execute as células de **`01_Reconhecimento_Facial.ipynb`** e
   **`02_Clusterizacao_Logistica_KMeans.ipynb`** na ordem apresentada.

---

##  Tecnologias Utilizadas

| Categoria              | Ferramentas                          |
| ---------------------- | ------------------------------------ |
| Linguagem              | Python 3.x                           |
| Visão Computacional    | OpenCV (Haar Cascade)                |
| Machine Learning       | scikit-learn (K-Means)               |
| Manipulação de Dados   | pandas, NumPy                        |
| Visualização           | Matplotlib                           |
| Ambiente               | Jupyter Notebook                     |

---

##  Documentação

O relatório técnico completo do projeto está disponível em
**`Relatorio_Melhores_Compras_Os_Mosqueteiros.pdf`**.

---

<p align="center">
  <img src="https://img.shields.io/badge/FIAP-Phase%206-ED145B?style=for-the-badge" alt="FIAP Phase 6"/>
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV"/>
  <img src="https://img.shields.io/badge/scikit--learn-K--Means-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="scikit-learn"/>
</p>



</p>
