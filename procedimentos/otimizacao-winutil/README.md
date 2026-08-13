# 🔧 Manutenção e ajustes do Windows com WinUtil

## 📌 Contexto

Durante uma prática de manutenção em meu ambiente Windows, utilizei o **WinUtil (Chris Titus Tech's Windows Utility)**, ferramenta open source voltada à configuração e manutenção do Windows.

A atividade foi realizada em ambiente próprio, com foco no aprofundamento de conhecimentos relacionados a suporte técnico e manutenção do sistema operacional.

## 🎯 Objetivo

Explorar recursos da ferramenta e realizar ajustes no ambiente Windows, observando configurações relacionadas ao funcionamento do sistema e ao consumo de recursos.

## 🛠️ Atividades realizadas

Durante a utilização do WinUtil, explorei recursos relacionados a:

* aplicativos e componentes instalados no Windows;
* programas e recursos executados em segundo plano;
* configurações do sistema operacional;
* recursos relacionados ao consumo de memória e processamento;
* manutenção e organização do ambiente Windows.


## 💻 Como realizar o procedimento

### 1. Abrir o Terminal como administrador

No Windows:

* clique com o botão direito no menu **Iniciar**;
* selecione **Terminal (Admin)** ou **Windows PowerShell (Admin)**.

Outra opção é pesquisar por `PowerShell` ou `Terminal` e utilizar **Ctrl + Shift + Enter** para executar como administrador.

> O WinUtil requer privilégios administrativos para realizar alterações no sistema.

### 2. Executar o WinUtil

No Terminal ou PowerShell aberto como administrador, execute o comando da versão estável:

```powershell
irm https://christitus.com/win | iex
```

Aguarde a inicialização da interface do WinUtil.

### 3. Analisar as opções disponíveis

Antes de aplicar alterações, revise as opções disponibilizadas pela ferramenta e avalie quais configurações são adequadas ao ambiente.

O WinUtil disponibiliza recursos relacionados a instalação de programas, ajustes do Windows, configurações, atualizações e outras tarefas de manutenção.

> Evite aplicar configurações sem compreender previamente o impacto que elas podem causar no sistema.

### 4. Aplicar as configurações

Selecione somente os ajustes que foram previamente analisados e são adequados ao objetivo da manutenção.

A ferramenta também disponibiliza configurações predefinidas (*presets*). A escolha deve considerar as necessidades do ambiente e os efeitos das alterações propostas.

### 5. Reiniciar e validar o ambiente

Após concluir as alterações:

1. reinicie o computador quando necessário;
2. verifique a inicialização do Windows;
3. valide o funcionamento dos aplicativos utilizados;
4. verifique conectividade e recursos necessários;
5. observe o comportamento e o consumo de recursos do sistema;
6. confirme se as alterações realizadas não afetaram funcionalidades necessárias.

Caso seja identificado algum comportamento inesperado, as alterações realizadas devem ser revisadas antes de novas modificações.


## 🔎 Validação

Após as alterações, acompanhei o comportamento do computador para observar os efeitos das configurações aplicadas e verificar o funcionamento do ambiente.

Não foi realizado um benchmark controlado antes e depois do procedimento. Portanto, esta documentação não atribui ganhos quantitativos de desempenho às alterações realizadas.

## 🧠 Aprendizados

A prática contribuiu para ampliar conhecimentos relacionados a:

* Windows;
* processos e serviços em segundo plano;
* consumo de recursos;
* manutenção preventiva;
* troubleshooting;
* análise de configurações;
* documentação técnica.

## 📷 Evidências

As evidências visuais do procedimento serão adicionadas neste diretório para registrar a ferramenta e os recursos utilizados durante a prática.

## ⚠️ Cuidados

Alterações em configurações do sistema operacional devem ser avaliadas antes da aplicação, considerando o ambiente, o impacto das mudanças e a possibilidade de reversão.

## 🔗 Ferramenta utilizada

**WinUtil — Chris Titus Tech's Windows Utility**

O WinUtil é uma ferramenta open source de terceiros e não foi desenvolvido por mim. Esta documentação registra exclusivamente minha utilização da ferramenta em ambiente próprio.

