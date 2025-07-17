# 📦 Tutorial: Criando uma Imagem com o Clonezilla

Este tutorial mostra como criar uma imagem de um sistema utilizando o Clonezilla, ideal para replicar uma máquina em múltiplos computadores. A seguir, estão os passos detalhados com instruções e espaços reservados para você inserir as capturas de tela.

---

## 1. Inicializando o Clonezilla

Após iniciar o computador com o Clonezilla no pendrive bootável, selecione a segunda opção:
> **Clonezilla live (VGA 800x600 & To RAM)**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/80b40a4f-48d9-4f3d-a3c1-bb8e499ded1f)

---

## 2. Escolha do Idioma

Selecione o idioma:  
> **pt_BR.UTF-8 Brazilian Portuguese | Português do Brasil**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/93a57e69-6bd8-45a8-80a8-0d7ebf4efe9a)

---

## 3. Layout do Teclado

Selecione:  
> **Keep - Manter layout de teclado padrão (layout US)**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/3a4f92bf-50bf-4408-939a-254762be03d1)

---

## 4. Iniciar o Clonezilla

Escolha:  
> **Start_Clonezilla - Iniciar Clonezilla**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/3cf8360c-0e23-428c-8d7a-ed91a09aafdc)

---

## 5. Modo de Operação

Escolha o modo:  
> **device-image - Trabalhar com imagens de disco/dispositivo**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/0e0c0b30-92ad-4bcd-ac0a-f0a1a2da6858)

---

## 6. Origem/Destino da Imagem

Selecione a opção:  
> **local_dev - Usar um dispositivo local (HD/pendrive externo)**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/5298a512-210d-44f0-8a4e-83eb5cae480a)

---

## 7. Conectar o Dispositivo de Armazenamento

Conecte o dispositivo USB onde a imagem será salva e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/e017807f-aea6-4f75-ab5b-7880c53bdc9a)

---

## 8. Listagem dos Dispositivos

O Clonezilla listará os dispositivos conectados.  
Aguarde o reconhecimento do dispositivo USB e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/1414e094-a15b-4bbd-9078-8e3aacecde48)

---

## 9. Selecionar Dispositivo de Armazenamento

Localize seu dispositivo na lista e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/87d30cc7-eea2-46dd-a333-92213dbb431e)

---

## 10. Verificação de Sistema de Arquivos

Escolha:  
> **no-fsck - Pular verificação do sistema de arquivos**  
e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/46d8fde1-51bc-4375-97cc-47ae8676a54e)

---

## 11. Selecionar Diretório para Salvar

Escolha o diretório onde deseja salvar a imagem (pode deixar na raiz) e selecione **done**.  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/67614af2-b1cd-4e40-86ab-3968ed738984)

---

## 12. Confirmação

O Clonezilla pedirá confirmação do caminho. Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/2243fa10-63bb-4131-886e-20a1a4245149)

---

## 13. Nome da Imagem

Digite o nome da imagem.  
💡 **Recomendação:** utilize o padrão: `data-tipo-marca`  
Exemplo: `2025-07-17-pc-lenovo`

![Image](https://github.com/user-attachments/assets/1db3e271-f78f-4f84-ab4e-ea9eec6ab501)

---

## 14. Selecionar Disco Fonte

Escolha o disco principal da máquina base e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/e59e159c-d28e-41c0-a5e0-b33f2c2b59a2)

---

## 15. Prioridade do Tipo de Backup

Selecione:  
> **-q2 - Prioridade: partclone > partimage > dd**

![Image](https://github.com/user-attachments/assets/fcec3a95-10c8-401c-af8d-e36cbe2aabc1)

---

## 16. Opções de Backup

Mantenha as opções padrão (ou ajuste conforme necessário).  
Para marcar/desmarcar, use a tecla **Espaço**.  
Depois pressione **Enter**.

![Image](https://github.com/user-attachments/assets/ccba3838-89e2-41e3-abcc-242abb225cd0)

---

## 17. Tipo de Compressão

Selecione o tipo de compressão:  
💡 Recomendado: `-z3` ou `-z6`  
São mais lentas na criação, mas excelentes na velocidade de clonagem.

![Image](https://github.com/user-attachments/assets/012a76b6-d59e-43b7-bee2-08f59dc48b43)

---

## 18. Tamanho Máximo por Volume

Para não dividir o arquivo da imagem:  
> Deixe o valor como `10000000` (equivale a "sem divisão").

![Image](https://github.com/user-attachments/assets/19195d31-8909-47f2-af6f-b8888b136cd0)

---

## 19. Verificação do Sistema de Arquivos de Origem

Escolha:  
> **-sfsck - Ignorar verificação/correção do sistema de arquivos de origem**

![Image](https://github.com/user-attachments/assets/cafd7e93-9143-445b-8afb-e074d8c4e827)

---

## 20. Verificação da Imagem Salva

Escolha:  
> **-scs - Não verificar a imagem salva**

![Image](https://github.com/user-attachments/assets/8de2b693-ceb5-4137-b456-eef52b1d8478)

---

## 21. Criptografia

Escolha:  
> **-senc - Não criptografar a imagem**

![Image](https://github.com/user-attachments/assets/75995dd9-f8e3-43e6-9b7e-c2acc6e14c83)

---

## 22. Ação Após o Processo

Escolha:  
> **-p choose - Perguntar o que fazer após o processo**  
Assim você poderá decidir entre desligar, reiniciar ou repetir.

![Image](https://github.com/user-attachments/assets/ebd0baf2-ce81-44d4-a974-c8063166f41a)

---

## ✅ Conclusão

Após confirmar, o processo de criação da imagem será iniciado.  
Acompanhe a barra de progresso na tela e **não mexa na máquina ou no dispositivo de armazenamento** até o término da operação.

---
