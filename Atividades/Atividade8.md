# Atividades do Módulo 3 - QA NA PRÁTICA 📚

Esse [repositório](https://github.com/LeanDevLima/Squad02_M3) é dedicado às atividades realizadas durante o Módulo 3 - QA NA PRÁTICA do curso de Quality Assurance oferecido pelo [**Instituto JogaJunto**](https://www.jogajuntoinstituto.org/). 

## 🚀 Descrição da 8ª Atividade: 🌟


🔍 ATIVIDADE: ESCREVENDO O CENÁRIO DE TESTE 
- Funcionalidade 1: Envio de áudio no WhatsApp; 
- Funcionalidade 2: Tirar uma selfie; 
 
Escreva os cenários de teste para as duas funcionalidades acima.

- A seguir, apresento um resumo das discussões em grupo, complementado por minhas contribuições adicionais:


___

Inicialmente, desenvolvemos cenários de teste levando em conta nossas experiências pessoais ao executar as tarefas mencionadas.
___

### Funcionalidade 1: Enviar um Áudio no WhatsApp


**Cenário 1: Enviar um áudio bem-sucedido**
1. Abrir o aplicativo WhatsApp.
2. Selecionar um contato válido da lista de contatos.
3. Clicar no ícone de anexo para abrir o menu de opções.
4. Escolher a opção "Áudio".
5. Gravar um áudio de 15 segundos.
6. Clicar no botão de envio.
7. Verificar se o áudio é exibido na janela de chat correta.
8. Verificar se o relógio de entrega indica a hora correta de envio.

**Cenário 2: Cancelar gravação de áudio**
1. Abrir o aplicativo WhatsApp.
2. Selecionar um contato válido da lista de contatos.
3. Clicar no ícone de anexo e escolher "Áudio".
4. Iniciar a gravação, mas em seguida, cancelar antes de concluir.
5. Verificar se a gravação foi cancelada e não enviada ao contato.

**Cenário 3: Envio de áudio sem rede**
1. Desativar a conexão de rede (Wi-Fi e dados móveis).
2. Abrir o aplicativo WhatsApp.
3. Selecionar um contato válido da lista de contatos.
4. Tentar enviar um áudio.
5. Verificar se o aplicativo exibe uma mensagem de erro relacionada à falta de conexão de rede.

**Cenário 4: Envio de áudio com tamanho máximo**
1. Abrir o aplicativo WhatsApp.
2. Selecionar um contato válido da lista de contatos.
3. Clicar no ícone de anexo e escolher "Áudio".
4. Gravar um áudio que atinja o tamanho máximo permitido (por exemplo, 5 minutos).
5. Tentar enviar o áudio.
6. Verificar se o aplicativo valida e impede o envio de áudios maiores que o limite.

### Funcionalidade 2: Tirar uma Selfie

**Cenário 1: Tirar uma selfie bem-sucedida**
1. Abrir o aplicativo da câmera.
2. Verificar se a câmera frontal está ativada.
3. Clicar no botão de captura para tirar a selfie.
4. Verificar se a imagem é exibida na tela de visualização.
5. Salvar a selfie.
6. Verificar se a selfie é salva corretamente na galeria de fotos.

**Cenário 2: Trocar para câmera traseira**
1. Abrir o aplicativo da câmera.
2. Verificar se a câmera frontal está ativada por padrão.
3. Trocar para a câmera traseira usando o botão apropriado.
4. Clicar no botão de captura para tirar uma foto.
5. Verificar se a imagem é exibida na tela de visualização.
6. Salvar a foto.
7. Verificar se a foto tirada com a câmera traseira é salva corretamente.

**Cenário 3: Aplicar filtro à selfie**
1. Abrir o aplicativo da câmera.
2. Verificar se a câmera frontal está ativada.
3. Acessar as opções de filtro disponíveis.
4. Escolher um filtro para aplicar à selfie.
5. Clicar no botão de captura para tirar a selfie com o filtro.
6. Verificar se a imagem filtrada é exibida na tela de visualização.
7. Salvar a selfie filtrada.
8. Verificar se a selfie com o filtro é salva corretamente na galeria.

**Cenário 4: Cancelar tirar selfie**
1. Abrir o aplicativo da câmera.
2. Verificar se a câmera frontal está ativada.
3. Clicar no botão de cancelar ou sair antes de tirar a selfie.
4. Verificar se a câmera é fechada sem tirar a foto.

<br>

___

Após adquirirmos uma compreensão mais profunda dos princípios do Desenvolvimento Orientado a Comportamento (BDD), reestruturamos os cenários de teste de acordo com esses conceitos.
___



### Funcionalidade 1: Enviar um Áudio no WhatsApp

- **Cenário: Enviar um áudio bem-sucedido**

__Dado que:__ o aplicativo WhatsApp está aberto; E um contato válido da lista de contatos foi selecionado;

__Quando:__ o usuário clica no ícone de anexo e escolhe a opção "Áudio"; E grava um áudio de 15 segundos, E clica no botão de envio;

__Então:__ o áudio deve ser exibido na janela de chat correta; E o relógio de entrega deve indicar a hora correta de envio;

- **Cenário: Cancelar gravação de áudio**

__Dado que:__ o aplicativo WhatsApp está aberto; E um contato válido da lista de contatos foi selecionado;

__Quando:__ o usuário clica no ícone de anexo e escolhe "Áudio"; E inicia a gravação, mas em seguida, cancela antes de concluir;

__Então:__ a gravação não deve ser enviada ao contato;

- **Cenário: Envio de áudio sem rede**

__Dado que:__ a conexão de rede está desativada; E o aplicativo WhatsApp está aberto; E um contato válido da lista de contatos foi selecionado;

__Quando:__ o usuário tenta enviar um áudio;

__Então:__ o aplicativo deve exibir uma mensagem de erro relacionada à falta de conexão de rede;

- **Cenário: Envio de áudio com tamanho máximo**
  
__Dado que:__ o aplicativo WhatsApp está aberto; E um contato válido da lista de contatos foi selecionado;

__Quando:__ o usuário clica no ícone de anexo e escolhe "Áudio"; E grava um áudio que atinge o tamanho máximo permitido; E tenta enviar o áudio;

__Então:__ o aplicativo deve validar e impedir o envio de áudios maiores que o limite;

### Funcionalidade 2: Tirar uma Selfie

- **Cenário - Tirar uma selfie bem-sucedida**
  
__Dado que:__ o aplicativo da câmera está aberto; E a câmera frontal está ativada;

__Quando:__ o usuário clica no botão de captura;

__Então:__ a imagem da selfie deve ser exibida na tela de visualização; E a selfie deve ser salva corretamente na galeria de fotos;

- **Cenário - Trocar para câmera traseira**
  
__Dado que:__ o aplicativo da câmera está aberto; E a câmera frontal está ativada por padrão;

__Quando:__ o usuário troca para a câmera traseira usando o botão apropriado; E clica no botão de captura para tirar uma foto;

__Então:__ a imagem da foto deve ser exibida na tela de visualização; E a foto tirada com a câmera traseira deve ser salva corretamente;


- **Cenário - Aplicar filtro à selfie**

__Dado que:__ o aplicativo da câmera está aberto; E a câmera frontal está ativada;

__Quando:__ o usuário acessa as opções de filtro disponíveis; E escolhe um filtro para aplicar à selfie
E clica no botão de captura para tirar a selfie com o filtro;

__Então:__ a imagem da selfie filtrada deve ser exibida na tela de visualização; E a selfie com o filtro deve ser salva corretamente na galeria;

- **Cenário - Cancelar tirar selfie**
  
__Dado que:__ o aplicativo da câmera está aberto; E a câmera frontal está ativada;

__Quando:__ o usuário clica no botão de cancelar ou sair antes de tirar a selfie;

__Então:__ a câmera não deve tirar a foto;


## Integrantes da Squad:

| Beatriz Souza  | [Bruno Soares](https://www.linkedin.com/in/bruno-soaresdev/)  | [Leanderson Lima](https://www.linkedin.com/in/leanderson-dias-de-lima/) | [Rebeca Borges](https://www.linkedin.com/in/rebecaborgess/) | Sara Cruz | 