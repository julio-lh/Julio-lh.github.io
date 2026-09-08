
## 1. Autenticar no GitHub

Abra o terminal no VS Code e execute:

```bash
gh auth login
```

Escolha:

```text
GitHub.com
HTTPS
Yes
Login with a web browser
```

O comando irá abrir o navegador. Faça login na sua conta do GitHub e autorize o acesso.

Para verificar se a autenticação funcionou:

```bash
gh auth status
```

---

## 2. Conectar a pasta ao repositório

Entre na pasta do projeto:

```bash
cd caminho/para/Julio-lh.github.io
```

Verifique se o repositório remoto já está configurado:

```bash
git remote -v
```

O resultado esperado é:

```text
origin  https://github.com/julio-lh/Julio-lh.github.io.git (fetch)
origin  https://github.com/julio-lh/Julio-lh.github.io.git (push)
```

### Se `origin` não existir

Execute:

```bash
git remote add origin https://github.com/julio-lh/Julio-lh.github.io.git
```

Depois confira novamente:

```bash
git remote -v
```

---

## 3. Enviar alterações para o GitHub

Depois de fazer alterações no projeto:

```bash
git add .
```

Faça o commit:

```bash
git commit -m "Update"
```

Envie para o GitHub:

```bash
git push
```
