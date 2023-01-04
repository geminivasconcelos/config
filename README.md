# Passo a Passo para configuração do ambiente de desenvolvimento



Informações referentes a configuração de cada projeto no ambiente de produção/servidores estará descrito nos seus respectivos repositórios

---

### Softwares utilizados para desenvolvimento

- Instalar [Oracle Client](https://download.oracle.com/otn_software/nt/instantclient/1911000/instantclient-basic-windows.x64-19.11.0.0.0dbru.zip)
  - Adicionar ao PATH (Windows)
- Instalar [Oracle JDK](https://www.oracle.com/br/java/technologies/javase-jdk11-downloads.html#license-lightbox)
  - Definir variável de ambiente JAVA_HOME (Windows)
- Instalar [Git](https://github.com/git-for-windows/git/releases/download)
- Instalar [VSCode](https://code.visualstudio.com/download)
- Instalar [Visual Studio Community](https://visualstudio.microsoft.com/pt-br/thank-you-downloading-visual-studio/?sku=Community&rel=16) (Apenas compiladores C++)
- Instalar [Python 3](https://www.python.org/ftp/python/3.8.10/python-3.8.10-amd64.exe)
  - Adicionar ao PATH (Windows)
- Instalar [Postman](https://www.postman.com/downloads/)
- Instalar [Windows Terminal](https://www.microsoft.com/pt-br/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab)
- Instalar (Dbeaver)[https://dbeaver.io/download/]
  - Configurar Conexões: Ver README_DB
- Instalar [NVM](https://github.com/coreybutler/nvm-windows)

  1. Instalar versão do node padrão utilizada:

     `nvm install 12.22.1`

  2. fechar e abrir novamente terminal e executar:

     `nvm use 12.22.1`

  3. Executar a instalação dos pacotes globais com o comando:

     `npm i -g @angular/cli pm2 typescript @nestjs/cli`

---

### Configuração de repositórios de versionamento e padrões a serem seguidos, instalação de depêndencias do projeto

1. Após clonar repositórios, `npm i` dentro de cada diretório para instalação das dependências de cada projeto

#### Regras para commit

- Usar commit atômico (diariamente) , e sempre sem erros que inviabilizam a execução da aplicação
- Usar commits imperativos, com a primeira letra em maiúsculo sempre tentando comunicar o que o commit faz sem que seja necessário olhar o conteúdo do commit
- Usar o corpo do commit para explicar "porquê", “para quê”, “como” (quando necessário) e detalhes adicionais
- Evitar commits com mensagens genéricas ou sem contexto: “Agora vai”, “Ajustado”, “Ajustado css”, “Fixado Isso”
