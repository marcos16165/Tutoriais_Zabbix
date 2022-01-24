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

Para testar o template, volte ao menu de ‘Configuração’ e selecione ’Hosts’. Na parte superior direita, selecione ‘create host’.
<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150828485-538ef218-f0a0-4cd4-952e-958e987aa861.png" />
</p>

Escolha um nome para o host, farei o teste com o site o UOL por isso nomeei como ‘URL UOL’, em seguida selecione ou crie um novo grupo. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150828506-12a74faf-f25c-4733-84e4-8d941fb97479.png" />
</p> 

Selecione e adicione o template.

Selecione e adicione o template.

<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150828525-a0527d97-076d-4104-a8f5-ad846817c215.png" />
</p> 

Agora vá até a opção ‘Macros’, preencha os campos, selecionando a opção ‘Change’. 
- **{$PORTAL} :** Nome do portal/site;
- **{$SITE_STRING} :** Busca uma palavra no corpo da página (Exemplo: nome do portal, palavra do cabeçalho e etc. Opte por palavras que estão na página de forma permanente, caso a palavra não seja encontrada, uma mensagem de erro é retornada, indicando que o site está offline); 
- **{$SITE_URL} :** URL a ser monitorado.

Após preencher os campos, clique em ‘Update’.
<p align="center">
  <img src="https://user-images.githubusercontent.com/38138237/150828548-df5e4649-f57f-4978-8055-678fc9654fa6.png" />
</p>  

