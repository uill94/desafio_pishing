PROJETO CRIAÇÃO DE UM PISHING COM O KALI LINUX
Através de uma ferramenta chamada setoolkit iremos criar uma página de login, que tem como objetivo capturar usuário e senha assim que digitado nos campos.

Ferramentas utilizadas no projeto:
- Oracle Virtual Box
- Kali Linux
- Setoolkit
Primeiramente antes de startar o sistema Kali Linux devemos realizar a configuração da placa de rede utilizada na máquina virtual a mesma tem que estar em modo Bridge,
 pois teremos que ter acesso a internet para realizar o projeto. Isso pode ser facilmente feito acessando as configurações da máquina virtual, e depois no campo “Rede”
selecionar o modo Bridge, feito isso podemos dar continuidade ao projeto.
 ![image](https://github.com/user-attachments/assets/46330364-0132-473f-981a-018ee1f11809)
![image](https://github.com/user-attachments/assets/84b61c7b-8885-4eb6-92e4-b70174698a85)

 

Abra sua máquina virtual Kali Linux, execute o comando “sudo su” no terminal, e depois chame a ferramenta “setoolkit”

![image](https://github.com/user-attachments/assets/9bf64482-1425-4e5a-ba33-2a78c36808f9)


 Selecione a opção “1” Soccial-Engineering Attacks.
 ![image](https://github.com/user-attachments/assets/dc1d52a5-b30b-40cc-8361-c78ad5d4e168)



Será exibido uma tela contendo várias opções de ataques, selecione a opção “2” Website Attack Vectors
![image](https://github.com/user-attachments/assets/80209594-76e6-4cdf-9043-bac35800e3b0)



Selecionamos a opção “3” Credential Harvester Attack Method
 ![image](https://github.com/user-attachments/assets/ddcf3c4f-c660-4403-bab6-863cc1a86c29)


Selecionamos a opção “2” Site Cloner
 ![image](https://github.com/user-attachments/assets/836d654b-3a0c-47be-bdd5-81963d8e8a5b)


Apertamos enter:
 
![image](https://github.com/user-attachments/assets/48b43356-b815-4149-b869-04dacd777705)

Agora temos que informar a url a ser clonada
 ![image](https://github.com/user-attachments/assets/4b0185ce-4776-405f-8609-d535bbf83a6d)


No exemplo usaremos a url do facebook.
![image](https://github.com/user-attachments/assets/4f190759-04af-4061-9020-7bd2b2a166b8)

 

Após digitar a url do facebook, o programa irá criar um servidor contendo um clone da pagina do facebook, e para acessar basta apenas digitar o ip 192.168.15.6 fornecido pela ferramenta.
![image](https://github.com/user-attachments/assets/c4ed8cf3-4221-4f3c-9c15-211384f61d8d)


 

Nesse momento você pode notar no terminal que houve um acesso a página fake.
![image](https://github.com/user-attachments/assets/5a1b8108-bcf2-4aa9-b44c-e9b8f8524870)

 

Agora com a pagina acessada, você digita seu login e senha para teste e o mesmo será capturado pelo pishing. No meu caso a pagina fake criada não da o glitch de captura 
igual mostrado ao instrutor mesmo fazendo todos os passos, mas teoricamente a captura dos dados aparecerá no terminal onde está sendo executada a ferramenta.


