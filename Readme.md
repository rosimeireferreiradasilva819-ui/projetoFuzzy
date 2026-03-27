# 💡 Sistema de Gorjeta com Lógica Fuzzy

Este projeto implementa um sistema baseado em **Lógica Fuzzy** utilizando a biblioteca `scikit-fuzzy` em Python.  
O objetivo é calcular o valor de uma gorjeta com base na qualidade da comida e do serviço.

---

## 📌 Sobre o Projeto

Em situações reais, nem sempre conseguimos definir valores exatos — por exemplo:  
"o serviço foi bom" ou "a comida estava ruim".

A lógica fuzzy permite trabalhar com essas incertezas, simulando decisões humanas.

Neste projeto:
- Entradas: qualidade da **comida** e do **serviço**
- Saída: valor da **gorjeta (%)**

---

## ⚙️ Tecnologias Utilizadas

- Python
- NumPy
- Matplotlib
- Scikit-Fuzzy

---

## 🧠 Como o Sistema Funciona

O sistema segue 4 etapas principais:

### 1. Definição das variáveis
- Comida (0 a 10)
- Serviço (0 a 10)
- Gorjeta (0 a 20)

### 2. Funções de pertinência
Cada variável é classificada em níveis:

**Comida:**
- Péssima
- Comível
- Deliciosa

**Serviço:**
- Ruim
- Aceitável
- Excelente

**Gorjeta:**
- Baixa
- Média
- Alta

---

### 3. Regras Fuzzy

O sistema possui regras como:

- Se comida é péssima e serviço é ruim → gorjeta baixa  
- Se comida é deliciosa e serviço é excelente → gorjeta alta  
- Se comida é comível e serviço é aceitável → gorjeta média  

No total, são utilizadas 9 regras.

---

### 4. Defuzzificação

Após aplicar as regras, o sistema converte o resultado fuzzy em um valor numérico real de gorjeta.

---

## ▶️ Como Executar

1. Instale as dependências:

```bash
pip install numpy matplotlib scikit-fuzzy