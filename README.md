# 🗂️ Flagr Dataroom

Este repositório contém o ambiente completo do **Data Room** da Flagr, baseado no [Nextcloud](https://nextcloud.com/), para uso em processos de Due Diligence.

---

## 🚀 O que está incluso

- Servidor Nextcloud com Docker  
- Banco de dados MariaDB  
- Volumes persistentes  
- Ambiente pronto para colaboração e controle de acesso por grupos  

---

## ✅ Requisitos

- Docker instalado  
- Git instalado  
- Acesso à internet  

---

## 🛠️ Como rodar o projeto localmente

1. **Clone o repositório**

```bash
git clone https://github.com/SEU_USUARIO/flagr-dataroom.git
cd flagr-dataroom
```

2. **Suba os containers com Docker Compose**

```bash
docker-compose up -d
```

3. **Acesse o Data Room pelo Navegador**

```bash
http://localhost:8080
```

4. **Configure o admin na primeira vez**

## -> Crie o usuário e senha de administrador.
## -> Use as seguintes credenciais de banco de dados:
    Usuário do banco: nextcloud  
    Senha do banco: senha_nextcloud  
    Nome do banco: nextcloud  
    Servidor do banco: db

---

## 🧱 Estrutura do Projeto

flagr-dataroom/
├── docker-compose.yml  # Configuração dos serviços
├── .gitignore          # Itens ignorados no Git
├── README.md           # Este guia

---

## 🧪 Comandos úteis

-> Ver logs do Nextcloud:

```bash
docker-compose logs -f app
```

-> Parar os containers:

```bash
docker-compose down
```

-> Subir novamente após alterações:

```bash
docker-compose up -d
```

---

## 🤝 Contribuição

-> Se for colaborar com alterações:

```bash
git checkout -b nome-da-sua-branch
# faça alterações...
git add .
git commit -m "Descreva sua alteração"
git push origin nome-da-sua-branch
```

---

## 🧩 Aplicativos recomendados para Data Room (Due Diligence)

-> Após o login como administrador no Nextcloud, instale os seguintes aplicativos através da interface "Aplicativos":

| Aplicativo                        | Descrição                                                                   |
| --------------------------------- | --------------------------------------------------------------------------- |
| **Group folders**                 | Cria pastas compartilhadas por grupos com controle granular de permissões.  |
| **File access control**           | Define regras de acesso a arquivos com base em grupo, IP, tags, etc.        |
| **Audit log**                     | Registra atividades do usuário para fins de auditoria e conformidade.       |
| **Activities**                    | Mostra histórico de ações em arquivos e pastas (uploads, downloads, etc).   |
| **Retention**                     | Define políticas de retenção e expiração de arquivos.                       |
| **Two-Factor TOTP Provider**      | Habilita autenticação em dois fatores com apps como Google Authenticator.   |
| **Password policy**               | Define regras mínimas para senhas dos usuários.                             |
| **End-to-end Encryption**         | Criptografa arquivos sensíveis para maior segurança.             |
| **Terms of service**              | Exibe e exige aceitação dos termos de uso para novos usuários.              |
| **Collaborative tags**            | Permite organizar e filtrar arquivos com tags visíveis por todos.           |
| **OnlyOffice / Collabora Online** | Permite visualização e edição de documentos direto no navegador. |

---

## 📬 Contato

Dúvidas? Fale com o time técnico da Flagr ou envie uma issue aqui no GitHub.