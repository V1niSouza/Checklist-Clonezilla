# 🖧 Clonagem de Imagem via Rede com Clonezilla (modo servidor)

Este tutorial orienta passo a passo como utilizar o Clonezilla em modo **servidor lite** para realizar a clonagem de uma imagem via rede (PXE boot), utilizando o próprio Clonezilla como servidor DHCP.

---

## 1. Inicialização do Clonezilla

Inicie o computador com o Clonezilla no pendrive bootável e selecione:

> **Clonezilla live (VGA 800x600 & To RAM)**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/80b40a4f-48d9-4f3d-a3c1-bb8e499ded1f)

---

## 2. Seleção de idioma

Escolha a linguagem:  
> **pt_BR.UTF-8 Brazilian Portuguese | Português do Brasil**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/93a57e69-6bd8-45a8-80a8-0d7ebf4efe9a)

---

## 3. Layout do teclado

Escolha:  
> **Keep layout de teclado padrão - layout US**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/3a4f92bf-50bf-4408-939a-254762be03d1)

---

## 4. Início do Clonezilla

Selecione:  
> **Start_Clonezilla Iniciar Clonezilla**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/3cf8360c-0e23-428c-8d7a-ed91a09aafdc)

---

## 5. Escolha do modo

Selecione:  
> **lite-server** (modo servidor Clonezilla)  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/252b8d70-ae79-4347-af2a-602aea11d837)

---

## 6. Início do servidor

Selecione:  
> **start Iniciar o servidor Clonezilla live lite**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/552b9dfe-6d57-43ab-9e77-7a3519a37a76)

---

## 7. Método de inicialização dos clientes

Escolha:  
> **netboot**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/1f949c9e-0663-458f-abfb-3b15c05234af)

---

## 8. Ambiente de rede

Escolha:  
> **start-new-dhcp** (Clonezilla gerará seu próprio DHCP)  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/50790f1e-7375-4e56-b1e9-1167bfd81a91)

---

## 9. Fonte da imagem

Escolha:  
> **local_dev**   
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/eb5427d3-a63a-4348-860d-3915f79f9f42)

---

## 10. Conecte o dispositivo USB com a imagem

Após conectar o USB, pressione **Enter**.

![Image](https://github.com/user-attachments/assets/ee5d3b26-2288-4532-bbcb-98418e5e7ad2)

---

## 11. Listagem de dispositivos

Aguarde a detecção ou reinserção.  
Quando aparecer, pressione **Ctrl + C**.

![Image](https://github.com/user-attachments/assets/1414e094-a15b-4bbd-9078-8e3aacecde48)

---

## 12. Selecione o dispositivo com a imagem

Escolha o armazenamento correto e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/87d30cc7-eea2-46dd-a333-92213dbb431e)

---

## 13. Montagem sem verificação

Selecione:  
> **no-fsck**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/46d8fde1-51bc-4375-97cc-47ae8676a54e)

---

## 14. Escolha a imagem

Selecione o diretório/arquivo da imagem.  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/b48746c0-eff6-4c3b-a7eb-08b9bec24a14)

---

## 15. Confirmação

Confirme com **Enter**.

![Image](https://github.com/user-attachments/assets/bb70a558-0a47-43b6-963d-3766d84030da)
---

## 16. Modo de execução

Escolha:  
> **Expert**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/15ab5fa6-165b-470a-9f32-85b9bae2d1cf)

---

## 17. Tipo de implementação

Escolha:  
> **massive-deployment**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/9739d385-3206-44ac-b851-c2978a96d6ca)

---

## 18. Tipo de origem da imagem

Escolha:  
> **from-image**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/ef29967c-181c-49cb-ad14-2fa490d11528)

---

## 19. Tipo de restauração

Escolha:  
> **restoredisk**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/099c728f-45d8-40ab-9630-0482da5a7168)

---

## 20. Escolha da imagem

Selecione a imagem correta para restauração.  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/d6a390ba-8b87-4c8a-bf19-e40189cab17d)

---

## 21. Disco de destino

Selecione o disco que será sobrescrito.  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/8ee801cd-20b6-4cf4-b985-701791372d05)

---

## 22. Parâmetros extras

Marque os necessários (ou mantenha padrão)  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/efdb5d0f-8820-445f-8c7e-3084290c833f)

---

## 23. Tipo de particionamento

Escolha:  
> **-k0** (usar esquema da imagem)  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/8004cad1-ab62-4414-93d1-35fc847fc750)

---

## 24. Verificação da imagem

Escolha:  
> **-sc0, pular verificação da imagem)**
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/3338ac60-4764-4352-a8ec-02ed68ca4c86)

---

## 25. Ação após restauração

Escolha:  
> **-p choose** (decidir depois)  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/152b3e19-5f41-4d54-b1b3-2780c8019599)

---

## 26. Tipo de restauração

Escolha:  
> **multicast**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/418cee11-381f-4585-aa90-3cf93e09e692)

---

## 27. Modo de espera

Escolha:  
> **clientes-to-wait**  
Pressione **Enter**.

![Image](https://github.com/user-attachments/assets/fad0d6ab-aac1-44f8-afd5-0abd23828e22)

---

## 28. Número de clientes

Digite a quantidade de máquinas a serem clonadas e pressione **Enter**.

![Image](https://github.com/user-attachments/assets/d1528e96-47f5-4adb-85d9-fae32f44ccd7)

---

Pronto! O servidor estará pronto para iniciar a clonagem assim que os clientes se conectarem via PXE. 🚀

---

## 📝 Observação

Agora com o servidor devidamente configurado, você pode iniciar suas máquinas clientes normalmente.  
⚠️ **Atenção!** Antes de ligar os computadores:

- Certifique-se de **conectar o cabo de rede**.
- Altere a **ordem de boot** na BIOS/UEFI para priorizar a inicialização via **PXE (Network Boot)**.

Assim, as máquinas conseguirão localizar o servidor Clonezilla e iniciar a clonagem automaticamente via rede.
