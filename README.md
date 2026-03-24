# base
Repositório Template para colocar a pasta resources no git.

Este repositório possui um arquivo `.gitignore` com os tipos de arquivos e diretórios que normalmente não são adicionados ao controle de versão.

## Como usar este repositório como template

Você pode criar um novo repositório a partir deste modelo de duas formas.

### Opção 1: Pelo botão **Use this template** (recomendado)

1. Abra este repositório no GitHub.
2. Clique em **Use this template**.
3. Selecione **Create a new repository**.
4. Defina:
	- Nome do novo repositório
	- Visibilidade (público/privado)
	- Organização ou conta de destino
5. Clique em **Create repository from template**.
6. Clone o novo repositório na sua máquina:

```bash
git clone https://github.com/<sua-conta>/<seu-novo-repo>.git
cd <seu-novo-repo>
```

### Opção 2: Via Git local (sem herdar histórico)

Use esta opção se você quiser iniciar um repo novo com os mesmos arquivos, mas sem vínculo de histórico com este template.

```bash
git clone https://github.com/<org-ou-conta>/base.git meu-novo-repo
cd meu-novo-repo
rm -rf .git
git init
git add .
git commit -m "chore: inicia projeto a partir do template base"
git branch -M main
git remote add origin https://github.com/<sua-conta>/<seu-novo-repo>.git
git push -u origin main
```

## Boas práticas após criar seu novo repositório

- Atualize este `README.md` com objetivo, instruções e stack do seu projeto.
- Revise o `.gitignore` para garantir que está adequado ao seu cenário.
- Configure proteções de branch e CI/CD, se necessário.