# Como Instalar o Lombok no Eclipse

Lombok é uma biblioteca Java que ajuda a reduzir o código boilerplate, fornecendo anotações que geram automaticamente métodos como `getters`, `setters`, `toString`, `equals`, entre outros. Para usar Lombok no Eclipse, é necessário instalar a biblioteca e configurá-la corretamente no IDE.

### Passos para instalar o Lombok no Eclipse:

## 1. Download do Lombok

- Acesse o site oficial do **Lombok**:
  [https://projectlombok.org](https://projectlombok.org)
  
- Na página inicial, clique no botão **Download** para baixar a versão mais recente do Lombok. O arquivo baixado será um `.jar` (por exemplo, `lombok.jar`).

![image](https://github.com/user-attachments/assets/dfdae52d-4786-43b7-8f9f-bf69beda2aa2)

## 2. Executar o Instalador do Lombok

Após o download, siga os passos abaixo:

1. Navegue até o diretório onde o arquivo `lombok.jar` foi baixado.
2. Execute o arquivo `.jar`. Você pode fazer isso de duas formas:
   - **Via interface gráfica**: Clique duas vezes no arquivo `lombok.jar`.
   - **Via terminal**: Navegue até o diretório onde o arquivo foi baixado e execute o seguinte comando:
     ```bash
     java -jar lombok.jar
     ```

3. O instalador do Lombok irá abrir uma janela. Ele detecta automaticamente as instalações do Eclipse presentes no seu sistema.
   - Se o caminho do Eclipse não for detectado automaticamente, clique em **Specify Location...** e selecione o executável do Eclipse (geralmente chamado `eclipse.exe` ou `eclipse` no Linux).

![image](https://github.com/user-attachments/assets/e54928e9-5d7a-498b-8d99-a7331296c189)

3.1 - Você pode encontrar o caminho do executável do Eclipse da seguinte forma:

3.1.1 - Abra o Eclipse => Help => About Eclipse IDE

![image](https://github.com/user-attachments/assets/6f308d9a-21b9-4766-8a22-56f931de749e)

3.1.2 - Clique na aba Configuration

![image](https://github.com/user-attachments/assets/ada157a2-878c-4366-ab48-cc14c198aec2)

3.1.3 - Procure por: **-showsplash**. O caminho onde está instalado o seu eclipse está logo após o **-showsplash**

3.1.4 - Após informar o caminho onde o Eclipse está instalado a ferramenta vai exibir um ícone do Eclipse:

![image](https://github.com/user-attachments/assets/cff2a43d-9df0-41cb-8519-55744fd80b70)

  
4. Clique no botão **Install/Update** para integrar o Lombok ao Eclipse.

5. Após a instalação, você verá uma mensagem indicando que o Lombok foi instalado com sucesso.

## 3. Verificar a Instalação do Lombok no Eclipse

Agora que o Lombok foi instalado, é necessário verificar se ele está funcionando corretamente no Eclipse:

1. **Reinicie o Eclipse**: Feche o Eclipse e abra-o novamente.
2. **Verifique se o Lombok está configurado**:
   - No menu superior do Eclipse, clique em `Help` > `About Eclipse IDE`.
   - Na janela de "About", você deve ver o ícone do **Lombok** ou uma referência ao Lombok, indicando que ele foi integrado corretamente ao IDE.

## 4. Adicionar Dependência do Lombok ao Projeto

Para usar o Lombok em um projeto Java, você precisa adicionar a biblioteca Lombok ao **classpath** do projeto.

### A. Se você estiver usando **Maven**:

Adicione a dependência do Lombok ao arquivo `pom.xml`:

```xml
<dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <version>1.18.28</version> <!-- Verifique a última versão no site oficial -->
    <scope>provided</scope>
</dependency>
