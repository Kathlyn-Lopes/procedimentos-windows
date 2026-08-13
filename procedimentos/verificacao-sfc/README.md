# 🛡️ Verificação de arquivos do sistema com SFC

## 📌 Contexto

O **System File Checker (SFC)** é uma ferramenta nativa do Windows utilizada para verificar a integridade dos arquivos protegidos do sistema e, quando possível, reparar arquivos corrompidos.

Este procedimento registra a utilização do comando `sfc /scannow` como prática de suporte e manutenção do Windows.

## 🎯 Objetivo

Verificar a integridade dos arquivos protegidos do sistema operacional e identificar possíveis arquivos corrompidos, permitindo que o próprio Windows realize o reparo quando possível.

## 🛠️ Atividade realizada

Execução do **System File Checker (SFC)** por meio do Prompt de Comando com privilégios administrativos.

Comando utilizado:

```cmd
sfc /scannow
```

## 💻 Como realizar o procedimento

### 1. Abrir o Prompt de Comando como administrador

No Windows:

1. abra o menu **Iniciar**;
2. pesquise por `cmd` ou **Prompt de Comando**;
3. clique com o botão direito em **Prompt de Comando**;
4. selecione **Executar como administrador**;
5. confirme a solicitação do Controle de Conta de Usuário, caso seja apresentada.

> A execução com privilégios administrativos é necessária para que o SFC consiga verificar e reparar os arquivos protegidos do sistema.

### 2. Executar a verificação

No Prompt de Comando aberto como administrador, execute:

```cmd
sfc /scannow
```

Pressione **Enter**.

### 3. Aguardar a conclusão

O Windows iniciará a verificação dos arquivos protegidos do sistema.

Aguarde até que o processo seja concluído.

> Evite fechar o Prompt de Comando durante a verificação.

### 4. Analisar o resultado

Após a conclusão, o SFC apresentará uma mensagem informando o resultado da verificação.

O resultado pode indicar, entre outras situações:

* que nenhuma violação de integridade foi encontrada;
* que arquivos corrompidos foram encontrados e reparados;
* que foram encontrados arquivos que não puderam ser reparados automaticamente.

A ação seguinte deve ser definida de acordo com o resultado apresentado pelo sistema.

## 🔎 Validação

Após a execução do procedimento:

1. verifique a mensagem apresentada pelo SFC;
2. confirme se foram identificados problemas de integridade;
3. verifique se o Windows informou que realizou reparos;
4. quando aplicável, reinicie o computador;
5. valide novamente o funcionamento do sistema ou o comportamento que motivou a verificação.

## 🧠 Aprendizados

Este procedimento envolve conhecimentos relacionados a:

* Windows;
* suporte técnico;
* troubleshooting;
* manutenção do sistema operacional;
* integridade de arquivos do sistema;
* utilização do Prompt de Comando;
* análise de resultados de diagnóstico.

## ⚠️ Cuidados

O resultado apresentado pelo SFC deve ser analisado antes de realizar procedimentos adicionais.

Caso a ferramenta informe que não conseguiu reparar determinados arquivos, o diagnóstico deve continuar utilizando procedimentos adequados ao problema identificado, evitando alterações no sistema sem análise prévia.

## 🔗 Referência

**System File Checker (SFC)** — ferramenta nativa do Microsoft Windows.

Para informações atualizadas sobre utilização, resultados e procedimentos de reparo, consulte a documentação oficial da Microsoft.
