#  Guia Prático de Clonezilla 

Este repositório é destinado a profissionais que buscam **eficiência e agilidade na clonagem de máquinas** em ambientes diversos, como laboratórios, empresas ou escolas.

Aqui você encontrará uma **explicação breve, objetiva e prática sobre como utilizar o Clonezilla**, um software open-source baseado em Debian GNU/Linux, amplamente utilizado para backup, restauração e clonagem de discos e partições.

---

## 📥 Sobre o Clonezilla

O Clonezilla é uma poderosa ferramenta de clonagem e recuperação de sistemas. Por ser open-source e baseada no Linux Debian, oferece uma alternativa robusta e gratuita a soluções comerciais, permitindo:

- Criar imagens completas de discos ou partições;
- Clonar máquinas via rede (multicast);
- Restaurar imagens em poucos minutos.

Você pode baixar a ISO oficial no site:  
🔗 [https://clonezilla.org/downloads.php](https://clonezilla.org/downloads.php)

⚠️ **Recomendo sempre utilizar a versão estável.**  
Após o download, utilize um programa como Rufus, Ventoy ou BalenaEtcher para criar um pendrive bootável com a ISO.

---

## 🧭 Estrutura do Repositório

Este repositório possui 3 branches adicionais, cada uma contendo um tutorial voltado para um cenário específico de uso do Clonezilla:

- [`tutorial-criando-imagem`](https://github.com/V1niSouza/Checklist-Clonezilla/tree/tutorial-criando-imagem?tab=readme-ov-file)  
  📦 Como criar uma imagem do sistema que será replicado

- [`tutorial-clonando-imagem-por-rede`](https://github.com/V1niSouza/Checklist-Clonezilla/tree/tutorial-clonando-imagem-por-rede?tab=readme-ov-file)  
  🌐 Clonagem de imagem via rede (modo servidor PXE)

- [`tutorial-clonando-imagem-apartir-de-um-hd-externo`](https://github.com/seu-user/seu-repo/tree/tutorial-clonando-imagem-apartir-de-um-hd-externo)  
  💽 Clonagem usando imagem salva em HD externo ou pendrive

---

## ⚠️ Cuidados Importantes Antes da Clonagem

### 1. 🖥️ Máquinas em Domínio
Se sua rede utiliza domínio (Active Directory), **não gere a imagem com a máquina base vinculada ao domínio**.  
Durante a clonagem, tudo será replicado, inclusive:
- O nome da máquina;
- A entrada no domínio.

Isso pode causar **conflitos de confiabilidade** e exigirá que as máquinas clonadas sejam reconectadas manualmente, uma por uma, ao domínio — o que compromete toda a automação do processo.

### 2. ⬆️ Atualizações e Licenciamento
Garanta que o sistema operacional e os softwares da máquina base estejam:
- Atualizados;
- Licenciados corretamente;
- Com configurações padrão desejadas.

Clonar uma máquina desatualizada fará com que você tenha retrabalho em todas as outras após a clonagem.

### 3. 🌐 DHCP e Ambiente de Rede

Se o ambiente onde será feita a clonagem via rede possui um **servidor DHCP ativo**, isole-o temporariamente, se possível.

O Clonezilla, em modo servidor (SE), oferece duas opções:

- Utilizar um **DHCP já existente** na rede;
- Ou **criar um novo servidor DHCP temporário**, que será iniciado junto com os demais serviços do Clonezilla SE (como TFTP e NFS).

⚠️ **Embora seja possível utilizar o DHCP existente**, **não é recomendado** fazer isso em redes em produção (ex: empresas, escolas ou setores em horário de expediente), pois o processo de clonagem consome largura de banda e pode causar **congestionamento na rede**, afetando outros setores e serviços.

💡 **Recomendação**: sempre que possível, use um switch isolado e conecte apenas as máquinas envolvidas no processo de clonagem.

---

## ✅ Considerações Finais

Este repositório é voltado para **uso técnico e direto ao ponto**, com foco em produtividade.  
A ideia é servir como material de consulta rápida para técnicos e administradores de redes que desejam aproveitar todo o potencial do Clonezilla com segurança e eficiência.

Contribuições são bem-vindas!

📫 Para dúvidas, sugestões ou colaborações, sinta-se à vontade para entrar em contato:  
[Vinicius Souza no LinkedIn](https://www.linkedin.com/in/vinisouza05/)


---

