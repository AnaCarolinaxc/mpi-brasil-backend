# MPI Brasil Backend

Backend da plataforma MPI Brasil.


---

## Instalação Windows

### Kotlin

1. **Instale o IntelliJ IDEA** (recomendadado, já inclui o compilador Kotlin):
   - Acesse [https://www.jetbrains.com/idea/download/](https://www.jetbrains.com/idea/download/)
   - Baixe a versão **Community** (gratuita)
   - Execute o instalador e siga as instruções na tela

2. **Ou instale o Kotlin manualmente via Chocolatey** (caso prefira linha de comando):
   ```powershell
   # Instale o Chocolatey caso ainda não tenha (execute como Administrador)
   Set-ExecutionPolicy Bypass -Scope Process -Force
   [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072
   iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

   # Instale o Kotlin
   choco install kotlinc
   ```

3. **Verifique a instalação:**
   ```powershell
   kotlinc -version
   ```

---

### PostgreSQL

1. **Baixe o instalador:**
   - Acesse [https://www.postgresql.org/download/windows/](https://www.postgresql.org/download/windows/)
   - Clique em **Download the installer** e escolha a versão mais recente

2. **Execute o instalador:**
   - Escolha o diretório de instalação
   - Selecione os componentes: **PostgreSQL Server**, **pgAdmin 4** e **Command Line Tools**
   - Defina a senha do usuário `postgres` 
   - Mantenha a porta padrão **5432**
   - Conclua a instalação

3. **Verifique a instalação:**
   ```powershell
   psql --version
   ```

4. **Conecte-se ao banco para testar:**
   ```powershell
   psql -U postgres
   ```
   Informe a senha definida durante a instalação quando solicitado.

---

## Instalação Linux