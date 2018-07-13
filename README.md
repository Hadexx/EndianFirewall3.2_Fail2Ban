# EndianFirewall3.5_Fail2Ban
Addon Fail2ban for Endian Firewall Community 3.2.x.

<br>

Versão:
--------

v.2.0 ( Testado no Endian Firewall Community na versão 3.2.5).

<br>

Requerimentos/opcional:
--------
- Requer: Acesso SSH ao Servidor e configuração de "Proxy SMTP" para o envio de alertas por e-mail.

<br>

<br>

Realizando download do pacote:
--------

Para realizar a compra/download do pacote acesse o site http://www.4nsecurity.com.br/loja/EndianFirewall_Fail2ban. 

Obs: O Arquivo pode ser enviado para o firewall atraves das ferramentas (winscp - para windows) ou atraves do scp no terminal linux.

<br>

<br>

Executando a instalação do pacote:
-------

No Terminal SSH do Servidor (com o usuario root) execute o comando abaixo:
    
    rpm -Uvh fail2ban-endian3-2.0-1.x86_64.rpm
    
<br>

Habilitando o Serviço:
-------

1 - Acesso o painel de controle do Endian Firewall com o usuario Admin, selecione o menu "Firewall" e em seguida o sub-menu "Fail2ban Protecao".
<br>
<br>
2 - Seleciona a caixa checkbox "Habilitar" e pressione o botão "Salvar" para que o serviço inicialize.
<br>
<br>
Obs: No menu estado voce podera vizualizar se o Serviço Fail2ban esta "em execução". 

<br>

Configuraçoẽs do Serviço:
--------

Tempo de BAN:
------
<br>

O Tempo de BAN é a difinição de quanto tempo (em Segundos) o IP atacante ficara banido no acesso aos serviços que esta sendo protegidos.

<br>

O valor padrão é de 3600 ( 1 hora ), os valores aceitos sao de -1 (para ban permanente) a 99999 (segundos).

<br>
<br>

Contador de BAN:
------
<br>

O Contador de BAN é a quantidade de falhas de login para e execução do BAN do IP atacante, seu valor padrão é de 5 tentativas e os valores aceitos sao de 1 a 99.

<br>

Removendo o pacote:
--------
- No console ssh digite:

    rpm -e fail2ban-endian3
    
  <br>  
    
Outras informações:
------------------



Espero ter ajudado.

Atenciosamente,

Bruno Almeida.
