# 🐚 Minishell - Construindo Seu Próprio Shell Unix

![C](https://img.shields.io/badge/Language-C-blue) ![Makefile](https://img.shields.io/badge/Build-Makefile-yellow) ![Readline](https://img.shields.io/badge/Library-Readline-orange) ![Norminette](https://img.shields.io/badge/Style-Norminette-green)

O projeto **Minishell** tem como objetivo criar um shell Unix básico, como o **Bash**, permitindo que os estudantes repliquem funcionalidades essenciais de um intérprete de comandos. Este projeto é uma oportunidade para explorar a fundo conceitos de programação de sistemas, manipulação de processos e controle de entrada e saída.

---

## 📋 Objetivo do Projeto

Desenvolver um shell Unix funcional que seja capaz de:
- **Executar comandos básicos**, como ls, echo, pwd, etc.  
- **Gerenciar variáveis de ambiente**, permitindo exportar, modificar e acessar valores.  
- **Lidar com redireções** (`>`, `>>`, `<`) e **tubos** (`|`) para conectar comandos.  
- Implementar **comandos internos**, como `cd`, `exit`, `env`, e `export`.  
- **Responder a sinais do sistema**, como Ctrl+C, Ctrl+D e Ctrl+\.  

Este projeto visa ensinar os conceitos fundamentais de programação de sistemas e como funciona um shell básico por trás dos panos.

---

## 📚 Conceitos Fundamentais

- **Gestão de Processos**: criação e manipulação de processos filhos com `fork()`, execução com `execve()`.  
- **Redireção e Tubos**: controle de entrada e saída com `dup2()` e conexão de comandos encadeados com pipes.  
- **Manipulação de Sinais**: tratamento de interrupções, como Ctrl+C, para garantir a estabilidade do shell.  
- **Biblioteca Readline**: leitura interativa de comandos e gerenciamento do histórico de entrada.  
- **Variáveis de Ambiente**: manipulação de variáveis globais usadas por processos no sistema Unix.  

---

## ✨ Funcionalidades Implementadas

### 🔧 Comandos Internos
1. **`echo`**: exibe uma mensagem no terminal, com suporte à flag `-n`.  
2. **`cd`**: muda o diretório atual para o especificado.  
3. **`pwd`**: exibe o diretório de trabalho atual.  
4. **`export`**: adiciona ou modifica variáveis de ambiente.  
5. **`unset`**: remove variáveis de ambiente.  
6. **`env`**: exibe todas as variáveis de ambiente disponíveis.  
7. **`exit`**: encerra o shell com um código de saída.

### ⚙️ Recursos Adicionais
- **Execução de Comandos Externos**: busca comandos no `$PATH` e executa programas binários.  
- **Suporte a Redireções**:
  - `>`: redireciona a saída padrão para um arquivo.  
  - `>>`: redireciona a saída padrão para o final de um arquivo.  
  - `<`: redireciona a entrada padrão a partir de um arquivo.  
- **Tuberias (`|`)**: conecta a saída de um comando à entrada de outro.  
- **Histórico de Comandos**: permite navegação e reutilização de comandos anteriores usando a biblioteca **Readline**.  
- **Tratamento de Sinais**:
  - Ctrl+C: interrompe o comando atual sem fechar o shell.  
  - Ctrl+D: encerra o shell se nenhuma entrada for fornecida.  
  - Ctrl+\: desabilitado para evitar encerramentos indesejados.  

---

## 🛠️ Ferramentas e Padrões

| Ferramenta/Padrão      | Descrição                                               |
|-------------------------|-------------------------------------------------------|
| **GIT**                | Controle de versão para organizar o desenvolvimento do código. |
| **Makefile**           | Automação da compilação e geração do executável.       |
| **Norminette**         | Garantia de conformidade com os padrões de estilo da 42. |
| **Biblioteca Readline**| Utilizada para leitura interativa e histórico de comandos. |

---

