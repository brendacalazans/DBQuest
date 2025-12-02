# 🤖 Configuração do Desafio de IA

O DBQuest possui um recurso de **Desafios SQL Gerados por IA** que cria perguntas personalizadas usando a API do Google Gemini.

---

## 🔑 Como Configurar a Chave de API

### Passo 1: Obter a Chave de API do Google Gemini

1. Acesse [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Faça login com sua conta Google
3. Clique em **"Get API Key"** ou **"Create API Key"**
4. Copie a chave gerada (formato: `AIza...`)

---

### Passo 2: Adicionar a Chave no Código

Abra o arquivo `src/scripts/app-full.jsx` e localize a linha (aproximadamente linha 2600):

```javascript
const GEMINI_API_KEY = ''; // Adicione sua chave aqui
```

Substitua por:

```javascript
const GEMINI_API_KEY = 'SUA_CHAVE_AQUI'; // Exemplo: 'AIzaSyC...'
```

---

### Passo 3: Salvar e Testar

1. Salve o arquivo
2. Recarregue a página no navegador
3. Clique em **"Desafio SQL"** no menu
4. O sistema deve gerar um desafio personalizado!

---

## ⚠️ **Importante: Segurança**

- **NÃO** compartilhe sua chave de API publicamente
- **NÃO** faça commit da chave no GitHub
- Para produção, use variáveis de ambiente ou um backend seguro

---

## 🐛 Solução de Problemas

### Erro: "Não foi possível gerar um desafio"

**Causa:** Chave de API não configurada ou inválida

**Solução:**
1. Verifique se a chave foi colada corretamente
2. Confirme que a chave está ativa no Google AI Studio
3. Verifique o console do navegador (F12) para ver o erro detalhado

---

### Erro: "Quota exceeded"

**Causa:** Você atingiu o limite gratuito da API

**Solução:**
- Aguarde até o próximo dia (o limite é resetado diariamente)
- Ou faça upgrade no Google Cloud Console

---

## 📚 Recursos Adicionais

- [Documentação do Gemini API](https://ai.google.dev/docs)
- [Limites de Uso Gratuito](https://ai.google.dev/pricing)

---

Desenvolvido com 💛 por @mayasrl
