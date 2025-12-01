

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
