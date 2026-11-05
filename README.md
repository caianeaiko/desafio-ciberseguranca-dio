# Desafio de Cibersegurança — DIO

## Objetivo
Realizar uma auditoria de segurança em ambiente controlado utilizando Kali Linux e Medusa, compreendendo ataques de força bruta e medidas de proteção.

## Ferramentas
- Kali Linux
- Oracle VirtualBox
- Medusa
- vsftpd (servidor FTP)

## Configuração do laboratório
O laboratório foi configurado em uma máquina virtual Kali Linux, utilizando um servidor FTP local para os testes.

## Etapas
1. Instalação do VirtualBox e Kali Linux.
2. Atualização do sistema.
3. Instalação e verificação do Medusa.
4. Instalação e configuração do vsftpd.
5. Verificação da conectividade com o servidor FTP local.
6. Documentação dos testes de auditoria.

## Evidências
As capturas de tela serão adicionadas à pasta images/.

## Medidas de mitigação
- Utilizar senhas fortes e únicas.
- Limitar tentativas de autenticação.
- Monitorar logs de acesso.
- Preferir SFTP ou FTPS ao FTP sem criptografia.

## Conclusão
O laboratório permitiu compreender a configuração de um ambiente de testes de segurança e a importância de proteger serviços de autenticação. Os resultados dos testes com Medusa serão documentados após sua execução.

## Teste de força bruta — FTP

Foi realizado um teste de autenticação em ambiente local controlado, utilizando Kali Linux, Medusa e o servidor vsftpd.

**Alvo:** 127.0.0.1 (localhost)

**Usuário de laboratório:** testeftp

**Ferramenta:** Medusa

**Resultado:** O Medusa identificou a senha de teste presente na wordlist, demonstrando o risco de utilizar senhas fracas.

### Evidência

![Resultado do teste FTP com Medusa](Images/medusa.png)

### Recomendações de segurança

- Utilizar senhas fortes e exclusivas.
- Implementar mecanismos de limitação de tentativas de login.
- Monitorar tentativas de autenticação malsucedidas.
- Preferir SFTP ou FTPS para proteger as credenciais durante a transmissão.
