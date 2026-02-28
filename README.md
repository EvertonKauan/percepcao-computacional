
---
## Se ainda não tem o ambiente conda instalado:

### 1. Download e Instalação

1. **Baixe o instalador:**
```bash
curl -O https://repo.anaconda.com/archive/Anaconda3-2023.09-0-Linux-x86_64.sh

```

2. **Execute o script:**
```bash
bash Anaconda3-2023.09-0-Linux-x86_64.sh

```
* Pressione **Enter** para ler os termos e digite `yes` para aceitar.
* Pressione **Enter** novamente para confirmar o local de instalação padrão.

3. **Inicialize o Conda:**
Quando o instalador perguntar se deseja rodar o `conda init`, digite `yes`. Isso configura as variáveis de ambiente automaticamente no seu `.bashrc`.
4. **Atualize o terminal:**
```bash
source ~/.bashrc

```
---

### 2. Gerenciando Ambientes

O Conda isola as bibliotecas para que as dependências de um projeto não quebrem as de outro.

### 3. Criando o ambiente e instalando dependências

* **Para criar o ambiente com Python 3.9.13:**
```bash
conda create -n percepcao python=3.9.13

```
* **Para ativar o ambiente e instalar o arquivo de requerimentos:**
Primeiro, ative o ambiente recém-criado:
```bash
conda activate percepcao
```

Em seguida, use o **pip** para instalar as dependências listadas no seu arquivo:
```bash
pip install -r requirements.txt

```
---

## Caso já tenha o ambiente conda instalado:

* **Para criar o ambiente com Python 3.9.13:**
```bash
conda create -n percepcao python=3.9.13

```

* **Para ativar o ambiente e instalar o arquivo de requerimentos:**
```bash
conda activate percepcao
```

Em seguida, use o **pip** para instalar as dependências listadas no seu arquivo:
```bash
pip install -r requirements.txt

```
---

* ** Para instalar o tensorflow e usar com a GPU:**

```bash
pip install "tensorflow[and-cuda]"
```