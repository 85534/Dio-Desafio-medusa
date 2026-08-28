# Dio-Desafio-medusa
Desafio de código ciberseguranca

# 🔐 Auditoria de Força Bruta com Kali Linux e Medusa

Projeto prático para demonstrar ataques de força bruta em serviços FTP, Web (DVWA) e SMB, utilizando **Kali Linux** e a ferramenta **Medusa**, em ambiente controlado com **Metasploitable 2** e **DVWA**.

## 📌 Objetivos

- Simular ataques de força bruta em serviços comuns.
- Utilizar o Medusa para automatizar tentativas de login.
- Documentar comandos, wordlists e resultados.
- Propor medidas de mitigação para cada vetor explorado.

## 🧰 Ambiente de Laboratório

| Componente         | Descrição                                  |
|--------------------|--------------------------------------------|
| VirtualBox         | Hipervisor para as VMs                     |
| Kali Linux         | Máquina atacante (IP: 192.168.56.101)      |
| Metasploitable 2   | Máquina alvo – serviços vulneráveis (IP: 192.168.56.102) |
| DVWA               | Aplicação web vulnerável instalada no Metasploitable ou em VM separada |
| Rede               | Host-Only (isolada)                        |

### Topologia

![Topologia](images/topologia.png)

## ⚙️ Configuração do Ambiente

1. Criar duas VMs no VirtualBox:
   - Kali Linux (imagem oficial).
   - Metasploitable 2 (imagem oficial).
2. Configurar ambas com adaptador de rede **Host-Only**.
3. Iniciar as VMs e verificar conectividade:
   ```bash
   ping 192.168.56.102
