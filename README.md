# Projeto ECOAR — Plataforma de Apoio a Alunos em Risco de Evasão

## 📘 Visão Geral

O **Projeto ECOAR** é uma plataforma desenvolvida para identificar, acompanhar e apoiar estudantes em risco de evasão acadêmica. Voltado para instituições de ensino superior, o sistema integra análise de dados, gestão de atendimentos e comunicação entre alunos, mentores e coordenação.

Seu objetivo principal é **reduzir a evasão**, oferecendo recursos que permitem ações preventivas, intervenções rápidas e monitoramento contínuo da jornada do aluno.

---

## 🎯 Objetivos do Sistema

* Identificar alunos com indicadores de risco (frequência, notas, engajamento, dificuldades pessoais).
* Facilitar o acompanhamento individual de cada estudante.
* Gerar relatórios e insights para gestores educacionais.
* Centralizar atendimentos e comunicações.
* Criar um ambiente seguro e acolhedor para o aluno.

---

## 🧩 Estrutura do Projeto

O projeto é dividido em dois módulos principais:

### **1. Backend (Flask)**

Localizado em `backend/`. Responsável por:

* APIs REST
* Processamento dos dados
* Regras de negócios
* Gestão dos registros dos alunos
* Dashboard administrativo

Principais arquivos:

* `app.py` — Inicialização da aplicação Flask.
* `core/ecoar.py` — Lógica do núcleo do sistema.
* `routes/api.py` — Endpoints de API.
* `routes/dashboard.py` — Rotas do dashboard.

### **2. Interface Inicial / Servidor (run.py)**

Localizado em `inicio/run.py`.

* Executa o servidor Flask.
* Roda em modo de desenvolvimento.
* Pode ser configurado para produção com Gunicorn/Nginx.

---

## 🚀 Como Executar o Projeto

### **Requisitos**

* Python 3.10+
* Pip
* Virtualenv (opcional, recomendado)

### **Passo a passo**

```bash
cd inicio
python run.py
```

O servidor iniciará em:

```
http://127.0.0.1:8000
```

---

## 🛠 Tecnologias Utilizadas

* **Python + Flask** — Backend e API.
* **HTML/CSS/JS** (se houver templates).
* **MongoDB** (dependendo da configuração do ambiente).
* Integrações futuras possíveis: dashboards externos, bots, IA.

---

## 📂 Funcionalidades Principais

### ✔ Cadastro e acompanhamento de alunos

Armazena dados básicos e indicadores de risco.

### ✔ Sistema de alertas

Gera sinalizações automáticas quando um aluno se aproxima de padrões de risco.

### ✔ Painel de controle para gestores

Exibe métricas gerais e casos que exigem atenção.

### ✔ Registro de atendimentos

Possibilita anotações, retornos, agendamentos e acompanhamento de suporte.

### ✔ Histórico completo do aluno

Permite ao gestor acompanhar a evolução do aluno ao longo do semestre.



## 📊 Possíveis Expansões Futuras

* Integração com Moodle/SIGAA.
* Análises com IA para prever evasão com maior precisão.
* Módulo de atendimento psicológico.
* App mobile.
* Envio automático de mensagens aos alunos.



