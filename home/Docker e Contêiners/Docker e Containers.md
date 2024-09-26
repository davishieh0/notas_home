Cliente    -> Servidor
(meu pc) -> (várias placas de vídeo)

## Conceitos importantes
- Bare Metal: Parte física, hardware
- Kernel: Parte central do SO que gerencia memória cpu e armazenamento

### Problemas com escala
Conforme as grandes aplicações web escalam, erros como problemas de ram, disco, problemas no código são frequentes.

Conforme seu servidor escala, ele pode crescer de **duas formas diferentes:**
### 1. Escalada Verticalmente
- Aumentar a RAM e CPU do próprio computador

### 2. Escalada Horizontalmente
- Aumentar o número de servidores menores
- divididos em **Microserviços**

-> Um problema é o Bare Metal, e a alocação de recursos, que muda de maquina p/ máquina e seus sistemas operacionais
- Usam-se **Máquinas virtuais** para resolver esse problema

- Alocação de Cpu e memória de uma MV ainda é fixa, resolvemos isso com **Docker:**

### Docker
- Todos compartilham o mesmo kernel de sistema operacional host 
- Alocam dinamicamente recursos com base na necessidade do sistema operacional
- Desenvolver software sem ter que fazer mudanças no sistema local

## Etapas do Docker
### 1. DockerFile
- Informa ao docker como configurar seu ambiente

### 2. Image
- arquivo docker é usado para construir uma imagem do seu sistema operacional, suas dependências e seu código.

### 3. Executar como um container
- Pacote isolado executando o código
- Quando desconectados, todos seus dados são perdidos

### 4. Mandar o container para a nuvem
- Aws,serviço de container elástico
- google cloud, sem servidor

### 5. Agora qualquer um pode acessar seu código sem ter que baixar milhões de coisas