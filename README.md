# Projeto EPTA - Comparação e análise de voo Nashira.
Projeto desenvolvido por mim para o desafio EPTA (EQUIPE DE PROPULSÃO E TECNOLOGIA AEROESPACIAL) da UFU.

# 🚀 Projeto EPTA - Desafio de Dinâmica de Voo: Calisto vs. Nashira

**Autor:** Gabriel Araujo Bicalho  
**Curso:** Engenharia de Controle e Automação

## 📋 Sobre o Projeto
Este projeto consiste na modelagem, simulação e validação da dinâmica de voo de foguetes experimentais. O objetivo central foi comparar os dados teóricos gerados via simulação (modelo **Calisto**) com os dados reais coletados por telemetria (foguete **Nashira**).

O trabalho aborda desde o tratamento de dados brutos (`.csv`) até a análise de eventos críticos de voo, como queima do motor, apogeu e abertura de paraquedas.

## 🛠️ Ferramentas Utilizadas
* **Python 3** (Linguagem base)
* **Jupyter Notebook** (Ambiente de desenvolvimento)
* **RocketPy**: Biblioteca avançada para simulação de trajetórias de foguetes de sondagem.
* **Pandas & NumPy**: Manipulação e tratamento de dados telemétricos.
* **Matplotlib**: Geração de gráficos comparativos de alta fidelidade.

## 📈 Etapas do Desenvolvimento

### 1. Modelagem do Calisto (Teórico)
Configuração completa do veículo utilizando o motor **Cesaroni M1670**, definindo:
* Parâmetros de massa e inércia.
* Aerodinâmica (aletas NACA, ogiva e corpo).
* Condições atmosféricas e de lançamento.

### 2. Processamento do Nashira (Experimental)
Análise do arquivo `nashira_telemetry.csv`, incluindo:
* Limpeza de ruído dos sensores de aceleração e pressão.
* Sincronização temporal com o momento do lançamento (*liftoff*).
* Extração da velocidade vertical através do gradiente de altitude.

### 3. Comparação de Resultados
Análise cruzada de três variáveis fundamentais:
* **Altitude:** Validação do apogeu projetado vs. alcançado.
* **Velocidade:** Estudo da aceleração máxima e frenagem aerodinâmica.
* **Aceleração:** Identificação das vibrações estruturais e tempo de queima do motor.



## 📊 Principais Conclusões
* O modelo teórico apresentou um erro percentual reduzido em relação ao apogeu real, validando o uso do **RocketPy**.
* Foram identificados eventos de ejeção de paraquedas através da variação brusca na aceleração vertical e taxa de descida.
* A experiência permitiu compreender as discrepâncias inerentes ao mundo real, como ventos locais e variações de empuxo nominal.

