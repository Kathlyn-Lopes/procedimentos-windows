# 💽 Verificação de disco com CHKDSK

## 📌 Contexto

O **CHKDSK (Check Disk)** é uma ferramenta nativa do Windows utilizada para verificar o sistema de arquivos e os metadados de uma unidade em busca de erros lógicos e físicos.

Este procedimento foi estudado como parte do aprofundamento de conhecimentos em **suporte técnico, diagnóstico e manutenção de ambientes Windows**.

## 🎯 Objetivo

Utilizar o CHKDSK para verificar a integridade do sistema de arquivos de uma unidade, identificar possíveis erros e compreender as opções disponíveis para correção e análise do disco.

## 🛠️ Atividade realizada

Utilização do **CHKDSK** por meio do Prompt de Comando com privilégios administrativos para análise de uma unidade do Windows.

## 💻 Como realizar o procedimento

### 1. Abrir o Prompt de Comando como administrador

No Windows:

1. abra o menu **Iniciar**;
2. pesquise por `cmd` ou **Prompt de Comando**;
3. clique com o botão direito em **Prompt de Comando**;
4. selecione **Executar como administrador**;
5. confirme a solicitação do Controle de Conta de Usuário, caso seja apresentada.

### 2. Identificar a unidade que será verificada

Antes da execução, confirme a letra correspondente à unidade que deseja analisar.

Em uma instalação comum do Windows, a unidade do sistema costuma ser identificada como `C:`, mas isso deve ser confirmado antes da execução.

### 3. Executar uma verificação

Para verificar a unidade `C:`, execute:

```cmd
chkdsk C:
```

Pressione **Enter** e aguarde a análise.

Sem parâmetros de correção, o CHKDSK verifica a unidade e apresenta informações sobre seu estado.

### 4. Correção de erros com `/f`

Quando houver necessidade de corrigir erros encontrados no sistema de arquivos, o CHKDSK disponibiliza o parâmetro `/f`:

```cmd
chkdsk C: /f
```

O parâmetro `/f` orienta o CHKDSK a corrigir erros encontrados no disco.

Se a unidade estiver em uso, o Windows poderá informar que não é possível bloqueá-la e perguntar se a verificação deve ser agendada para a próxima inicialização.

### 5. Verificação com `/r`

Para localizar setores defeituosos e tentar recuperar informações legíveis, existe o parâmetro `/r`:

```cmd
chkdsk C: /r
```

O parâmetro `/r` inclui as funcionalidades do `/f` e realiza uma análise mais abrangente da unidade.

> A execução com `/r` pode levar um período considerável, principalmente em unidades maiores. Esse parâmetro deve ser utilizado quando houver uma necessidade de diagnóstico que justifique uma verificação mais profunda.

## 🔎 Validação

Após a execução:

1. analise o resultado apresentado pelo CHKDSK;
2. verifique se foram identificados erros no sistema de arquivos;
3. observe se o Windows informou a realização de correções;
4. caso a verificação tenha sido agendada, aguarde sua execução durante a reinicialização;
5. após a conclusão, valide o funcionamento normal do sistema.

## 🧠 Aprendizados

Este procedimento contribui para conhecimentos relacionados a:

* Windows;
* suporte técnico;
* troubleshooting;
* sistema de arquivos;
* diagnóstico de unidades;
* manutenção do sistema operacional;
* utilização do Prompt de Comando;
* análise de resultados de diagnóstico.

## ⚠️ Cuidados

Antes de utilizar parâmetros que realizam correções, é importante compreender o problema que está sendo investigado e confirmar a unidade selecionada.

Procedimentos de diagnóstico e reparo de armazenamento devem considerar a importância dos dados existentes na unidade e a disponibilidade de backup.

O processo não deve ser interrompido durante uma operação de correção.

## 🔗 Referência

**CHKDSK — Microsoft Windows**

* **Documentação oficial:** [chkdsk — Microsoft Learn](https://learn.microsoft.com/pt-br/windows-server/administration/windows-commands/chkdsk)

O CHKDSK é uma ferramenta nativa do Microsoft Windows.

Para parâmetros, comportamentos e orientações atualizadas, consulte a documentação oficial da Microsoft.
