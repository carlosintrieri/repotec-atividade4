
# 🏝️ Atlantis Water Park - Sistema de Gestão de Resort

Sistema completo de gestão para o resort fictício **Atlantis Water Park**, desenvolvido com React + TypeScript + Vite.

> **Nota**: Este projeto utiliza **localStorage** do navegador para armazenar todos os dados localmente. Não requer backend ou banco de dados externo.

## 📋 Sobre o Projeto

O Atlantis Water Park é um sistema de gerenciamento de resort que permite:

- ✅ **Cadastro de Clientes Titulares**: Registro completo de hóspedes principais
- ✅ **Cadastro de Dependentes**: Adicione dependentes vinculados ao titular
- ✅ **Gestão de Dados Pessoais**: CPF, RG, Passaporte, telefones com DDD e endereços completos
- ✅ **Seleção de Quartos**: Escolha de acomodações disponíveis no resort
- ✅ **Área de Clientes**: Painel para visualizar hóspedes atualmente hospedados no resort
- ✅ **Sistema de Check-out**: Realize check-out de clientes que estão no resort
- ✅ **Área de Hospedagens**: Histórico completo de check-ins e check-outs

## 🛠️ Tecnologias Utilizadas

- **React 18** - Biblioteca para construção de interfaces
- **TypeScript** - Tipagem estática para JavaScript
- **Vite** - Build tool moderna e rápida
- **Tailwind CSS** - Framework CSS utilitário
- **Lucide React** - Ícones modernos
- **localStorage** - Armazenamento local de dados no navegador

## 📦 Instalação

### Pré-requisitos
- Node.js (versão 16 ou superior)
- npm ou yarn

### Passo a passo

```bash
# Clone o repositório
git clone https://github.com/carlosintrieri/repotec-atividade4
cd repotec-atividade4

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

O aplicativo estará disponível em `http://localhost:5173`

## 💾 Armazenamento de Dados

O sistema utiliza o **localStorage** do navegador para armazenar todos os dados localmente. Isso significa que:

- ✅ Não precisa de servidor backend
- ✅ Não precisa de banco de dados externo
- ✅ Todos os dados ficam armazenados no seu navegador
- ⚠️ Os dados são específicos do navegador (não sincronizam entre dispositivos)
- ⚠️ Limpar dados do navegador apagará todos os registros

### Estrutura de Dados no localStorage

Os dados são organizados em diferentes chaves:

- **`clientes`**: Lista de clientes titulares e dependentes
- **`documentos`**: CPF, RG e Passaportes dos clientes
- **`telefones`**: Telefones com DDD vinculados aos clientes
- **`enderecos`**: Endereços completos dos clientes
- **`hospedagens`**: Registro de check-ins e check-outs
- **`quartos`**: Disponibilidade e status dos quartos

## 🎯 Funcionalidades Detalhadas

### 1. Cadastro de Clientes
- Formulário completo com validação
- Campos: Nome, email, data de nascimento
- Vinculação automática de documentos e contatos

### 2. Gestão de Dependentes
- Adicione dependentes ao cadastro do titular
- Cada dependente mantém seus próprios documentos e dados

### 3. Sistema de Documentos
- CPF (formato: XXX.XXX.XXX-XX)
- RG (formato: XX.XXX.XXX-X)
- Passaporte (alfanumérico)
- Validação de formatos

### 4. Telefones
- DDD + Número
- Suporte a múltiplos telefones
- Validação de formato brasileiro

### 5. Endereços
- CEP com busca automática (ViaCEP)
- Campos: Rua, número, complemento, bairro, cidade, estado
- Validação de campos obrigatórios

### 6. Seleção de Quartos
- Visualização de quartos disponíveis
- Tipos: Standard, Deluxe, Suíte
- Capacidade e comodidades

### 7. Check-in / Check-out
- Registro automático de datas
- Atualização de status de ocupação
- Histórico completo de estadias

### 8. Área de Clientes
- Lista de hóspedes atualmente no resort
- Informações de quarto e estadia
- Função de check-out rápido

## 🚀 Comandos Disponíveis

```bash
# Desenvolvimento
npm run dev          # Inicia o servidor de desenvolvimento (http://localhost:5173)

# Build
npm run build        # Compila o projeto para produção

# Preview
npm run preview      # Visualiza o build de produção localmente
```

## 📝 Licença

Este projeto é fictício e foi desenvolvido para fins educacionais e de demonstração.

---

<div align="center">
  <p>Desenvolvido com ❤️ para o Atlantis Water Park</p>
  <p>🏝️ Onde cada estadia é uma aventura! 🌊</p>
</div>
```sh
# Rodar:
npm i

# E depois:
npm run dev
```


# Passo a passo de como rodar o código:

# npm install lucide-react  
# npm install @types/react @types/react-dom  

# Dependências de desenvolvimento:
# npm install @types/node                
# npm install tailwindcss postcss autoprefixer  # Tailwind CSS + ferramentas para processar e otimizar o CSS
# npx tailwindcss init -p      

# npm install typescript @types/react @types/react-dom

# npm install react-scripts


# ===============================================================================
# INSTRUÇÕES FINAIS - CÓDIGO VITE + MYSQL + SEQUELIZE COMPLETO:
# ===============================================================================
#
# 1. COLE AS 3 PARTES EM SEQUÊNCIA no seu AtlantisWaterPark.jsx
# 2. CERTIFIQUE-SE que backend/server.js está rodando: node backend/server.js
# 3. EXECUTE o Vite: npm run dev  
# 4. ACESSE: http://localhost:5173 (ou porta do seu Vite)
#
# RESULTADO: Visual e layout 100% idênticos + dados no MySQL via Sequelize
# 
# ✅ Clientes titulares → tabela Clientes (titular_id = null)
# ✅ Dependentes → tabela Clientes (titular_id = ID do titular)  
# ✅ Documentos CPF/RG/Passaporte → tabela Documentos
# ✅ Telefones com DDD → tabela Telefones  
# ✅ Endereços completos → tabela Enderecos
# ✅ Check-ins/Check-outs → tabela Hospedagens
# ✅ Relacionamentos via Foreign Keys
#
# VERIFICAR NO MYSQL WORKBENCH:
# SELECT * FROM Clientes WHERE titular_id IS NULL;     -- Titulares
# SELECT * FROM Clientes WHERE titular_id IS NOT NULL; -- Dependentes  
# SELECT * FROM Documentos;                            -- Documentos
# SELECT * FROM Hospedagens;                           -- Hospedagens
#
# Sistema completo: Vite + React + TypeScript + Tailwind + MySQL + Sequelize!
