# 🌐 Diagnóstico de conectividade de rede no Windows

## 📌 Contexto

Problemas de conectividade podem estar relacionados a diferentes fatores, como configuração de rede, comunicação com o gateway, resolução de nomes ou instabilidade na conexão.

Este procedimento registra a utilização de ferramentas nativas do Windows para consultar configurações de rede e realizar testes básicos de conectividade durante atividades de troubleshooting.

## 🎯 Objetivo

Consultar informações da configuração de rede e realizar testes de comunicação para auxiliar na identificação de possíveis problemas de conectividade.

## 🛠️ Ferramentas utilizadas

* **IPCONFIG** — consulta informações da configuração TCP/IP do computador.
* **PING** — testa a comunicação com outro host e permite observar as respostas recebidas e o tempo de resposta.

## 💻 Como realizar o procedimento

### 1. Abrir o Prompt de Comando

No Windows:

1. abra o menu **Iniciar**;
2. pesquise por `cmd` ou **Prompt de Comando**;
3. abra o Prompt de Comando.

Para alguns comandos administrativos, pode ser necessário utilizar **Executar como administrador**.

### 2. Consultar a configuração de rede

Execute:

```cmd id="shx6yc"
ipconfig
```

O comando apresenta informações básicas das interfaces de rede, como endereço IPv4, máscara de sub-rede e gateway padrão.

Essas informações auxiliam na identificação da configuração atual de rede do computador.

### 3. Consultar informações detalhadas

Para obter informações adicionais, execute:

```cmd id="3lyrpf"
ipconfig /all
```

A saída apresenta detalhes adicionais das interfaces, que podem incluir:

* endereço IPv4;
* endereço físico (MAC);
* máscara de sub-rede;
* gateway padrão;
* servidores DNS;
* DHCP;
* informações relacionadas à concessão DHCP.

### 4. Testar conectividade com PING

Para verificar a comunicação com um destino, utilize:

```cmd id="hheqfv"
ping google.com
```

O comando envia solicitações ao destino e apresenta informações sobre as respostas recebidas.

Durante a análise, observe principalmente:

* respostas recebidas;
* tempo de resposta;
* pacotes enviados;
* pacotes recebidos;
* perda de pacotes.

### 5. Realizar teste contínuo de conectividade

Para acompanhar a comunicação durante um período maior, utilize:

```cmd id="w0pb6g"
ping google.com -t
```

No Windows, o parâmetro `-t` mantém o teste em execução continuamente.

Esse teste pode auxiliar na observação de comportamentos como:

* interrupções momentâneas;
* perda de pacotes;
* ausência de resposta;
* variações no tempo de resposta.

Para interromper o teste, pressione:

```text id="lmy6h4"
Ctrl + C
```

Ao interromper, o comando apresenta as estatísticas do teste realizado.

## 🔎 Interpretação básica

### Respostas recebidas

Quando o destino responde, existe comunicação entre o computador e o endereço testado naquele momento.

### Tempo de resposta

O valor apresentado em `ms` representa o tempo de ida e volta da comunicação.

Variações devem ser analisadas considerando o tipo de conexão, o destino e as condições da rede.

### Perda de pacotes

A ocorrência de perda de pacotes durante testes sucessivos pode indicar a necessidade de investigar a conectividade.

O `ping` isoladamente não determina a causa do problema. Ele funciona como uma das evidências utilizadas durante o diagnóstico.

## 🔎 Validação

Durante o troubleshooting:

1. consulte a configuração de rede com `ipconfig`;
2. utilize `ipconfig /all` quando precisar de informações mais detalhadas;
3. realize um teste de comunicação com `ping`;
4. quando necessário, utilize `ping -t` para observar a conexão durante um período maior;
5. analise respostas, tempos e possíveis perdas de pacotes;
6. utilize os resultados como apoio para definir as próximas etapas do diagnóstico.

## 🧠 Conhecimentos relacionados

* Windows;
* suporte técnico;
* troubleshooting;
* redes;
* TCP/IP;
* DNS;
* DHCP;
* análise de conectividade;
* Prompt de Comando.

## ⚠️ Cuidados

A ausência de resposta a um `ping` não significa necessariamente que o equipamento ou serviço esteja indisponível, pois respostas ICMP podem ser bloqueadas por configurações de firewall ou pela própria infraestrutura.

Da mesma forma, variações de latência ou perda de pacotes devem ser analisadas em conjunto com outras informações antes de determinar a causa de uma instabilidade.

## 🔗 Referências

**IPCONFIG e PING — Microsoft Windows**

* [ipconfig — Microsoft Learn](https://learn.microsoft.com/windows-server/administration/windows-commands/ipconfig)
* [ping — Microsoft Learn](https://learn.microsoft.com/windows-server/administration/windows-commands/ping)

Para parâmetros e comportamentos atualizados dos comandos, consulte a documentação oficial da Microsoft.
