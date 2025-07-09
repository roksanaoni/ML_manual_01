{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyNjfHJECorSi5XfK+jz40Fw",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/roksanaoni/ML_manual_01/blob/main/%20README.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Fnk_CFS6FXLS",
        "outputId": "37a9ef7c-7edf-431a-8878-0d7795da5336"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Writing README.md\n"
          ]
        }
      ],
      "source": [
        "# 🩺 Diabetes Prediction using Linear Regression\n",
        "\n",
        "This project predicts whether a patient has diabetes using **Linear Regression** based on the Pima Indians Diabetes dataset.\n",
        "\n",
        "## 📌 Objective\n",
        "Build a linear regression model that takes clinical data and predicts a binary diabetes outcome (0 or 1). Though linear regression is not typically used for classification, this project adapts it for binary prediction by rounding the predicted values.\n",
        "\n",
        "---\n",
        "\n",
        "## 📂 Dataset\n",
        "\n",
        "The dataset contains 768 records with the following features:\n",
        "\n",
        "- Pregnancies\n",
        "- Glucose\n",
        "- BloodPressure\n",
        "- SkinThickness\n",
        "- Insulin\n",
        "- BMI\n",
        "- DiabetesPedigreeFunction\n",
        "- Age\n",
        "- Outcome (target: 0 = non-diabetic, 1 = diabetic)\n",
        "\n",
        "Source: [Pima Indians Diabetes Dataset (Kaggle)](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)\n",
        "\n",
        "---\n",
        "\n",
        "## ⚙️ Preprocessing Steps\n",
        "\n",
        "1. Replace all zero values in key features (`Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, `BMI`) with the **mean** or **median** of the column.\n",
        "2. Replace the **first row's Glucose** value with the **maximum Glucose** value in the dataset.\n",
        "3. For all records with the **minimum age**, replace their Glucose values with the **minimum Glucose** value from the dataset.\n",
        "\n",
        "---\n",
        "\n",
        "## 🧠 Model\n",
        "\n",
        "- Algorithm: **Linear Regression** (`sklearn.linear_model.LinearRegression`)\n",
        "- Predictions were **rounded to 0 or 1** to simulate classification.\n",
        "- Evaluated using standard classification metrics.\n",
        "\n",
        "---\n",
        "\n",
        "## 📊 Evaluation Metrics\n",
        "\n",
        "- **Accuracy**\n",
        "- **Precision**\n",
        "- **Recall**\n",
        "- **F1-Score**\n",
        "- **Confusion Matrix**\n",
        "\n",
        "These metrics are calculated using:\n",
        "```python\n",
        "from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, confusion_matrix\n"
      ]
    }
  ]
}