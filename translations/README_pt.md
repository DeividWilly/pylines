# decorationLine #

O **decorationLine** é uma bibloteca onde sua utilidade é decorar o seu programa Python que interaja no terminal.

> Este projeto é _open-source_ e está livre para distribuição e modificações, para saber mais verifique os termos e condições da licença [GNU GPLv3](https://github.com/DeividWilly/pylines/blob/main/LICENSE).
_ _ _
# Sumário #

* Guia de instalação
    * PIP
        * Windows
        * Linux
    * Biblioteca _decorationLine_
* Como usar

* Como colaborar

_ _ _

## Guia de instalação

### **PIP**
O **_PIP_** é um sistema de gerenciamento de pacotes para gerenciar bibliotecaas de software em Python. Os arquivos são armazenados no repositório online **_Python Package Index (PyPI)_**.

Por padrão, o **pip** vai procurar os pacotes e suas dependências no repositório **_PyPI_**, mas também é possível instalar seus pacotes diretamento do código fonte.
_ _ _
### Windows:

Baixe o arquivo **get-pip.py** e armazene-o no mesmo diretório que o **Python** está instalado.

Pelo CMD, abra o diretório onde os arquivos se encontram e digite o seguinte comando:
```bash
python3 get-pip.py
```
Para verificar se a instalação foi feita com sucesso, faça o comando:
```bash
pip -V
```
O CMD retornará a versão instalado no sistema.

_ _ _

### Linux 

No Debian, Ubuntu e derivados:
```bash
sudo apt-get install python-pip
```

Em distribuições baseadas em Arch Linux:
```bash
sudo pacman -S python-pip
```

Para mais outras distribuições, consulte com seus respectivos sistemas.

_ _ _

### **Biblioteca decorationLine** ###

Para instalar a biblioteca **decorationLine** é apenas necessário rodar o comando no terminal:

```bash
pip3 install decorationLine
```

_ _ _

### Como usar

Para usar é simples, a função `printLine()` necessita de alguns argumentos para funcionar, por exemplo:

```py
printLine(
    type=2, #Tipo de linha
    amount=15, #Quantidade
    backgroundColor='yellow', #Cor de fundo
    color='green', #Cor da caractere
    reverse=False, #De traz para frente
    end=False) #Quebra de linha
```
Saída:

![](/assets/images/example-output.png)

Há alguns tipos de linhas, cores e cores de fundo disponíveis. Você pode ver no código-fonte ou aqui mesmo:

```python
colors = {
	'clear': '\033[m',
	'black': '\033[30m',
	'red': '\033[31m',
	'green': '\033[32m',
	'yellow': '\033[33m',
	'blue': '\033[34m',
	'magenta': '\033[35m',
	'cyan': '\033[36m',
	'white': '\033[37m'
}
```
```python
backgroundColors = {
	'black': '\033[40m',
	'red': '\033[41m',
	'green': '\033[42m',
	'yellow': '\033[43m',
	'blue': '\033[44m',
	'magenta': '\033[45m',
	'cyan': '\033[46m',
	'white': '\033[47m'
}
```
```python
types = {
	1:'--',
	2:'=-',
	3:'*-',
	4:'==',
	5:'++',
	6:'**',
	7:'+-'
}
```
Para chamar o argumento certo da função, basta apenas inserir o valor certo na posição de cada variável.

## Como colaborar

Abra uma issue e reporte bugs ou também pode reportá-los no `bugs_found.txt`.

