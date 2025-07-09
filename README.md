{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyNfNb1Nwh5zWf3TXW3HIzG3",
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
        "<a href=\"https://colab.research.google.com/github/roksanaoni/ML_manual_01/blob/main/README.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": 1,
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
        "1. Title\n",
        "Diabetes Prediction using Linear Regression\n",
        "\n",
        "2. Objective\n",
        "To develop a machine learning model using Linear Regression for predicting diabetes outcomes (0 or 1) based on clinical features. The model will be trained on a diabetes dataset after proper preprocessing and evaluated using classification metrics.\n",
        "\n",
        "3. Introduction\n",
        "Diabetes is a growing global health concern. Predicting whether a person is diabetic based on clinical measurements can aid in early diagnosis and management. Although Linear Regression is typically used for continuous values, we apply it here to a binary classification task by rounding the predictions.\n",
        "\n",
        "4. Dataset\n",
        "We use the Pima Indians Diabetes Dataset, which includes 8 features such as Glucose, BMI, Age, etc., and a binary target variable Outcome.\n",
        "\n",
        "5. Preprocessing\n",
        "To ensure data quality, the following preprocessing steps were taken:\n",
        "\n",
        "Zero values in columns like Glucose, BloodPressure, BMI, etc., were replaced with the mean or median of the respective column.\n",
        "\n",
        "The first row's glucose value was replaced with the maximum glucose value in the dataset.\n",
        "\n",
        "For all records with the lowest age, their glucose values were replaced with the minimum glucose value from the dataset.\n",
        "\n",
        "6. Model Theory: Linear Regression\n",
        "Linear Regression tries to model the relationship between the dependent variable (Y) and one or more independent variables (X) by fitting a linear equation:\n",
        "\n",
        "𝑌=𝛽0+𝛽1𝑋1+𝛽2𝑋2+...+𝛽𝑛𝑋𝑛+𝜖Y=β0+β1X1+β2X2+...+βnXn+ϵ\n"
      ]
    }
  ]
}