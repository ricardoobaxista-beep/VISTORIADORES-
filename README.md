# 📊 BEQ — Dashboard de Vistoriadores

Dashboard de controle e gestão de vistoriadores da Região Metropolitana de Fortaleza.

## 🌐 Acesso Online

> **URL do GitHub Pages:**  
> `https://SEU_USUARIO.github.io/beq-dashboard/`

---

## 🚀 Como publicar no GitHub Pages

### 1. Criar o repositório

1. Acesse [github.com](https://github.com) e faça login
2. Clique em **"New repository"** (botão verde)
3. Preencha:
   - **Repository name:** `beq-dashboard`
   - **Visibility:** Public *(necessário para GitHub Pages gratuito)*
   - Deixe as demais opções como estão
4. Clique em **"Create repository"**

---

### 2. Fazer upload dos arquivos

**Opção A — Pelo navegador (mais simples):**

1. No repositório criado, clique em **"uploading an existing file"**
2. Arraste ou selecione os arquivos desta pasta:
   - `index.html`
   - `README.md`
3. Role até o fim da página e clique em **"Commit changes"**

**Opção B — Via Git (linha de comando):**

```bash
git init
git add .
git commit -m "primeiro commit — dashboard BEQ"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/beq-dashboard.git
git push -u origin main
```

---

### 3. Ativar o GitHub Pages

1. No repositório, clique na aba **"Settings"**
2. No menu lateral, clique em **"Pages"**
3. Em **"Source"**, selecione:
   - Branch: `main`
   - Pasta: `/ (root)`
4. Clique em **"Save"**
5. Aguarde ~1 minuto e acesse a URL exibida

---

## 🔄 Atualizar o dashboard

Sempre que gerar uma nova versão do arquivo HTML:

1. Renomeie o arquivo para `index.html`
2. No repositório GitHub, clique no arquivo `index.html`
3. Clique no ícone de lápis ✏️ (editar) **ou** faça upload do novo arquivo
4. Confirme com **"Commit changes"**

O site atualiza automaticamente em ~1 minuto.

---

## 📋 Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| 📊 Painel Produção | KPIs, gráficos e tabela detalhada por vistoriador |
| 🚫 Painel Cancelados | Análise completa de vistorias canceladas com filtros |
| 📂 Atualizar Base | Importa arquivo `.xlsx` local |
| 🔄 Sincronizar | Busca dados diretamente do Google Sheets |
| 📸 Export PNG | Salva gráficos e tabelas como imagem |
| 🗺️ Mapa RMF | Animação dos municípios da Região Metropolitana |

---

## ⚙️ Configuração do Google Sheets (Sincronização Online)

Para usar o botão **Sincronizar**, a planilha precisa estar publicada:

1. Abra a planilha no Google Sheets
2. Vá em **Arquivo → Compartilhar → Publicar na Web**
3. Selecione a aba desejada e formato **CSV**
4. Copie a URL gerada
5. Cole no arquivo `index.html` nas constantes:
   ```js
   const SHEET_MAIN_URL   = 'SUA_URL_ABA_RETORNOS';
   const SHEET_CANCEL_URL = 'SUA_URL_ABA_ACOMPANHAMENTO';
   ```

---

## 🛠️ Desenvolvido por

**Ricardo Lucas** — Gestão & Analytics  
© 2026 BEQ
