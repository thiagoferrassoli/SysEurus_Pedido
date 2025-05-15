# SysEurus Lista - Gerador de Listas a partir do SysEurus Consumo

**Descrição:**

O SysEurus Lista é um aplicativo complementar projetado para extrair e gerar listas com base nos dados inseridos no SysEurus Consumo. Ele facilita a organização e a utilização das informações de consumo registradas, permitindo a criação de relatórios, inventários ou outros tipos de listagens para análise ou uso em outros sistemas.

**Funcionalidades Principais:**

* **Geração de Listas a partir do SysEurus Consumo:** Extrai dados de consumo previamente registrados no SysEurus Consumo.
* **Interface de Configuração:** Oferece opções para selecionar os dados específicos a serem incluídos nas listas (por exemplo, produtos consumidos em um período, quantidades, usuários, etc.).
* **Flexibilidade de Formato:** Permite gerar listas em diferentes formatos (por exemplo, CSV, TXT) para facilitar a análise e a importação em outras ferramentas.
* **Visualização Prévia:** (Se aplicável) Oferece uma prévia da lista antes da exportação.
* **Foco na Análise de Consumo:** Desenvolvido para auxiliar na organização e análise dos dados de consumo registrados no SysEurus Consumo.

**Instalação:**

Para instalar o SysEurus Lista, siga os passos abaixo:

1.  **Descompactação:** Descompacte todo o conteúdo do pacote de instalação dentro da pasta:
    ```
    C:\Program Files (x86)\
    ```
2.  **Permissões de Edição para Todos os Usuários:** Após a descompactação, é necessário conceder permissões de edição (leitura e gravação) para todos os usuários do Windows à pasta do sistema. Isso garante que diferentes contas de usuário possam executar o aplicativo e salvar as listas geradas ou arquivos de configuração.

    * **Opção 1 (Interface Gráfica):**
        1.  Navegue até a pasta `C:\Program Files (x86)\` no Explorador de Arquivos.
        2.  Clique com o botão direito na pasta do SysEurus Lista (o nome da pasta pode variar).
        3.  Selecione "Propriedades".
        4.  Clique na aba "Segurança".
        5.  Clique no botão "Editar".
        6.  Na lista de "Nomes de grupo ou de usuário", selecione "Todos". Se "Todos" não estiver listado, clique em "Adicionar...", digite "Todos" e clique em "OK".
        7.  Na seção "Permissões para Todos", certifique-se de que as caixas de seleção "Leitura" e "Gravação" estejam marcadas. Você pode também marcar outras permissões relevantes, mas "Leitura" e "Gravação" são essenciais para a edição de arquivos de configuração ou para salvar logs.
        8.  Clique em "Aplicar" e depois em "OK" em todas as janelas abertas.

    * **Opção 2 (Linha de Comando - Executar como Administrador):**
        Abra o Prompt de Comando como administrador e execute o seguinte comando, substituindo `<NomeDaPastaDoSysEurusLista>` pelo nome real da pasta do SysEurus Lista:
        ```
        icacls "C:\Program Files (x86)\<NomeDaPastaDoSysEurusLista>" /grant Todos:(OI)(CI)M
        ```
        Este comando concede permissões de "Modificação" (`M`), que incluem leitura e gravação, de forma recursiva (`(OI)(CI)`) para todos os usuários (`Todos`).

**Utilização:**

Após a instalação e configuração das permissões, o SysEurus Lista estará pronto para gerar listas a partir dos dados do SysEurus Consumo.

1.  **Execute o SysEurus Lista.** O executável principal estará dentro da pasta onde você descompactou os arquivos em `C:\Program Files (x86)\`.
2.  **Conecte-se ao SysEurus Consumo:** (Se necessário) Configure a conexão com a base de dados ou arquivos de dados do SysEurus Consumo. Consulte a documentação do SysEurus Lista para detalhes sobre a configuração da conexão.
3.  **Selecione os dados:** Utilize a interface do aplicativo para escolher os dados específicos do SysEurus Consumo que você deseja incluir na lista.
4.  **Configure o formato:** Escolha o formato de saída desejado para a lista (por exemplo, CSV, TXT).
5.  **Gere a lista:** Execute a função de geração da lista.
6.  **Utilize a lista:** A lista gerada estará pronta para ser utilizada para análise, relatórios ou importação em outros sistemas, incluindo o SysEurus Pedido (se aplicável).

**Observações:**

* Certifique-se de que o SysEurus Consumo esteja instalado e contendo os dados de consumo desejados.
* A forma como o SysEurus Lista se conecta e extrai os dados do SysEurus Consumo dependerá da arquitetura de ambos os aplicativos. Consulte a documentação de ambos para obter detalhes sobre a integração.
* As permissões de edição são necessárias para que o aplicativo possa salvar arquivos de configuração ou logs.

**Suporte:**

Para suporte técnico ou dúvidas sobre a utilização do SysEurus Lista, entre em contato com a equipe de desenvolvimento ou o administrador do sistema.
