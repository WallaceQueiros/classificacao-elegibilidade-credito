# Classificação de Elegibilidade de Crédito

## 📘 Descrição
Este projeto utiliza um modelo supervisionado de classificação **KNN** para prever a elegibilidade de uma solicitação de crédito bancário nos EUA. O modelo classifica cada solicitação em uma das três categorias:

- **1 = Não Elegível**
- **2 = Elegível com Análise**
- **3 = Elegível**

---

## 🤖 Tipo de Modelo
- Modelo: **K-Nearest Neighbors (KNN)**
- Valor de K utilizado: **[inserir valor aqui, ex: 7]**

---

## 🔢 Variáveis utilizadas no modelo
As variáveis (features) utilizadas, em ordem no vetor de entrada, são:

1. `salario_anual` (Salário anual em dólares)
2. `total_dividas` (Total de dívidas em dólares)
3. `score` (Histórico de pagamento — valor entre 0 e 1)
4. `idade` (Idade do solicitante)

---

## ⚖️ Normalização
- As variáveis foram normalizadas utilizando o `StandardScaler` da biblioteca `sklearn.preprocessing`.
- O scaler utilizado está salvo no arquivo `scaler_knn.joblib`.

---

## 🧪 Exemplo de previsão real
- Entrada (X): `[45000, 15000, 0.85, 35]`  
- Saída (y): `[2]`  
  Isso significa que a solicitação foi classificada como **"Elegível com Análise"**.

---

## 📁 Arquivos incluídos
- `modelo_knn.joblib`: Arquivo com o modelo KNN treinado.
- `scaler_knn.joblib`: Objeto de normalização dos dados.

---

## 📌 Observações
- O modelo foi treinado com validação e ajuste de hiperparâmetro `K`.
- O dataset original foi pré-processado para garantir desempenho consistente.

