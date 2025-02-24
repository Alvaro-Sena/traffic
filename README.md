# Classificador de Sinais de Trânsito com Redes Neurais

Este projeto implementa um **classificador de sinais de trânsito** utilizando conceitos de **redes neurais convolucionais (CNN)**. Desenvolvido como parte do curso **CS50 - Introduction to Artificial Intelligence with Python**, oferecido pela **Harvard University**, o sistema é capaz de reconhecer e classificar 43 diferentes categorias de placas de trânsito.

## Tecnologias Utilizadas 

- **Linguagem**: Python 3.11  
- **Bibliotecas**: TensorFlow, Keras, OpenCV, scikit-learn
- **Ferramentas**: Git
- **Conceitos de IA**: Redes Neurais Convolucionais, Pré-processamento de Imagens, Transfer Learning

## Estrutura do Projeto

A pasta contém os seguintes arquivos:

- **`traffic.py`**: Implementação do modelo de classificação
- **`gtsrb/`**: Dataset com imagens de placas (43 categorias)
- **`requirements.txt`**: Dependências do projeto

## Features  
- Pré-processamento de imagens com redimensionamento e normalização
- Arquitetura CNN com camadas convolucionais e max-pooling
- reinamento com otimização Adam e dropout para prevenção de overfitting
- Avaliação de desempenho com métricas de acurácia
- Sistema de salvamento do modelo treinado

## Minha Contribuição

Desenvolvi toda a pipeline de machine learning no arquivo traffic.py, incluindo:
- Pré-processamento de imagens com redimensionamento e normalização
- Arquitetura CNN com camadas convolucionais e max-pooling
- Treinamento com otimização Adam e dropout para prevenção de overfitting
- Avaliação de desempenho com métricas de acurácia
- Sistema de salvamento do modelo treinado

## Como Funciona a Rede Neural

O sistema segue estas etapas principais:

1. **Carregamento de Dados**:
- Lê imagens do diretório gtsrb organizado em subpastas por categoria.
- Redimensiona imagens para 30x30 pixels.
2. **Pré-processamento**: 
- Converte imagens para arrays numpy.
- Normaliza valores de pixel (0-255 para 0-1).
3. **Modelo CNN**: 
- 2 camadas convolucionais com ativação ReLU.
- Camadas de Max-Pooling para redução dimensional.
- Camada densa final com ativação softmax para classificação.
4. **Treinamento**: 
- 10 épocas de treinamento com validação automática.
- Loss function: Categorical Crossentropy.
- Otimizador: Adam


## Instalação e Execução

1. Clone o repositório:  
   ```bash  
   git clone https://github.com/Alvaro-Sena/traffic.git  
   ```
2. Navegue até a pasta do repositório:
   ```bash  
   cd traffic/
   ``` 
3. Instale as dependências:  
   ```bash  
   pip install -r requirements.txt  
   ```
4. Baixe a pasta com os parâmetros:
   ```bash  
   curl -O https://cdn.cs50.net/ai/2023/x/projects/5/gtsrb.zip
   ```
5. Extraia a pasta:
   ```bash  
   unzip gtsrb.zip
   ```  
6. Execute o analisador:  
   ```bash  
   python traffic.py gtsrb 
   ```  

Certifique-se de que possui **Python 3** instalado no seu ambiente. Além disso, é necessário instalaçao das bibliotecas de requirements.txt.
É recomendado 4GB+ de RAM para treinamento da Rede Neural.

## Contato
Caso tenha dúvidas ou sugestões, entre em contato através do meu [LinkedIn](www.linkedin.com/in/alvaro-sena), [GitHub](https://github.com/Alvaro-Sena) ou [WhatsApp](https://wa.me/447356040385).
