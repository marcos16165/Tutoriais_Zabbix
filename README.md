## Observação
Antes de iniciar o tutorial, é importante ter o Zabbix instalado e configurado, para isso basta seguir os tutoriais disponibilizados no [zabbix.com](https://www.zabbix.com/documentation/5.2/pt/manual/installation/instal).

## Instalação do Template 

O template ‘Template Web Monitoring’, monitora sites para verificar se a página está online e retorna outras informações como:

- Tempo de resposta;
- Última mensagem de erro do cenário "Web";
- Failed step of scenario "Web";
- Velocidade de download.

Para instalar o template, siga os passos abaixo. 

### **1. Download e Importação:**
Após fazer download do arquivo ‘Template Web Monitoring’, disponível neste repositório.\
Para importar, basta abrir o zabbix, acessar o menu de ‘Configuration’ e escolher a opção ‘Templates’.

<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150812418-cb879c44-2a90-4703-bc92-f368316fbdfb.png" />
</p>

Em seguida, selecione a opção ‘import’ na parte superior direita. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150812422-b3ebafe4-ce0a-4a48-8b93-a2f4aab9cc0a.png" />
</p> 

Agora busque o arquivo baixado em seu computador. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150812425-5186d638-2e67-47dd-b4b3-73d7e274824d.png" />
</p> 

Por fim, selecione a opção ‘Import’

<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150812427-b7442c94-48fc-4870-9ee3-2fd72cdb4df6.png" />
</p> 

O template foi importado com sucesso, 

### **2. Testando o Template:**

Para testar o template é preciso ter um host já configurado, caso não saiba fazer isso acesse, [zabbix.com](https://www.zabbix.com/documentation/3.0/pt/manual/config/hosts/host). 
