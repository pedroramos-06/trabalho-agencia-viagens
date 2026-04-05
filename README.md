# ✈️ Agência de Viagens

Simulação de um site de agência de turismo com pacotes e destinos.

---

## 📄 Páginas obrigatórias

- **index.html** — apresentação da agência
- **destinos.html** — cards com imagens e vídeos dos lugares
- **tabela_precos.html** — tabela comparativa de pacotes
- **reserva.html** — formulário completo com datas, cidade e tipo de viagem
- **contato.html** — iframe do Google Maps + links para redes sociais

---

## 🧩 Elementos obrigatórios do tema

- Cards com imagens dos destinos
- Botões com ícones do framework
- `<select>` com cidades e pacotes
- Uso de `<video>` com poster

---

## ✅ Requisitos gerais

- Mínimo de 5 páginas HTML
- Um arquivo CSS externo ou sistema de classes do framework
- Menu de navegação funcional entre páginas
- Estrutura responsiva (com uso de grid ou flexbox do framework)
- Formulário completo
- Tabelas, listas, imagens, áudio ou vídeo
- Links internos e externos
- Uso real do framework (menus prontos, botões, cards, modais, etc.)
- Organização em pastas: `/css`, `/img`, `/audio`, `/video`

---

# 🔀 Fluxo de trabalho com Git

Guia rápido para todos do grupo seguirem o mesmo processo.

---

## 📋 Regras combinadas

- **Todo o código do projeto deve ficar dentro da pasta `src/`**
- **Nunca commite direto na `main`** — sempre via Pull Request
- **Sempre atualize a `main`** antes de começar uma tarefa nova
- **Outra pessoa deve revisar e aprovar** o Pull Request antes do merge
- **Uma branch por tarefa** — não misture coisas diferentes na mesma branch

---

## 🏷️ Prefixos — nomenclatura padrão

Tanto branches quanto commits usam prefixos para deixar claro o tipo de trabalho. Os mais comuns são:

| Prefixo | Quando usar |
|---|---|
| `feat/` | Nova funcionalidade |
| `fix/` | Correção de bug |
| `style/` | Mudança visual sem lógica |
| `docs/` | Documentação |

O formato é sempre `prefixo/descricao-curta`. A descrição usa hífen no lugar de espaço.

---

## 🚀 Começando uma tarefa nova

```bash
# 1. Entre na main e atualize
git checkout main
git pull

# 2. Crie sua branch com um nome descritivo
git checkout -b feat/nome-da-sua-tarefa
```

> **Exemplos de nome de branch:** `feat/navbar`, `feat/pagina-contato`, `fix/botao-quebrado`

---

## 💾 Salvando seu progresso (commits)

```bash
# Veja o que mudou
git status

# Adicione os arquivos modificados
git add .

# Salve com uma mensagem descritiva
git commit -m "feat: descrição curta do que foi feito"
```

> **Prefixos para mensagens de commit:**
> - `feat:` → nova funcionalidade
> - `fix:` → correção de bug
> - `style:` → mudança visual sem lógica
> - `docs:` → documentação

---

## ☁️ Subindo para o GitHub

```bash
# Primeira vez que sobe ESSA branch
git push origin feat/nome-da-sua-tarefa

# Nas vezes seguintes
git push
```

---

## 🔁 Abrindo um Pull Request (PR)

1. Após o `git push`, acesse o repositório no GitHub
2. Clique no botão **"Compare & pull request"** que aparece automaticamente
3. Escreva um título e uma breve descrição do que foi feito
4. Confirme que os campos estão corretos: `base: main` ← `compare: feat/sua-branch`
5. Clique em **"Create pull request"**
6. Avise o grupo para alguém revisar e aprovar

---

## ✅ Após o merge ser aprovado

```bash
# Volte para a main e atualize
git checkout main
git pull

# Delete a branch localmente (ela já cumpriu o papel)
git branch -d feat/nome-da-sua-tarefa
```

> ⚠️ **Por enquanto ignore a parte de deletar a branch.** Conforme o grupo ganhar mais confiança com o fluxo, isso pode ser adotado depois.

---

## 🔄 Resumo do ciclo completo

```
git checkout main
git pull
git checkout -b feat/minha-tarefa

# ... trabalha ...

git add .
git commit -m "feat: o que foi feito"
git push origin feat/minha-tarefa

# Abre o PR no GitHub → colega revisa → merge feito

git checkout main
git pull
git branch -d feat/minha-tarefa
```
