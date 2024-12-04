# Testes de Funcionalidades - Tabela de gerenciamento de usuários - Cãodominio 🐾

Este documento descreve os testes a serem realizados na tabela de gerenciamento de usuários e permissões de novos usuários do sistema **Cãodominio**. 

## 📂 Informações do Projeto

- **GitHub:** [Repositório do Projeto](https://github.com/quallifica-tech/caodominio/tree/develop)  
- **Figma:** [Design no Figma](https://www.figma.com/design/f2A5s87LxLyVfra0bjv8RB/ONGS?node-id=331-211&m=dev)

### Credenciais de Teste

- **Conta de Teste:** 
  - E-mail: `teste@teste.com`  
  - Senha: `teste123`
- **Conta de Admin:**  
  - E-mail: `admin@admin.com`  
  - Senha: `admin123`  
  *(Cada conta deve ser configurada com uma role específica.)*

---

## 🔍 Checkpoints para Testes

## Escopo do teste

1. **Acesso à Tabela de Usuários:**
   - Verificar se usuários com a role de admin conseguem acessar a tabela de gerenciamento de usuários. ✅
   - Confirmar que usuários sem a role de admin não têm acesso à tabela. ✅

2. **Criação de Novos Usuários:**
   - Testar a funcionalidade de criação de novos usuários, preenchendo todos os campos obrigatórios e verificar se o usuário é adicionado corretamente à tabela. ✅
   - Validar a criação de usuários com dados inválidos (ex: e-mail em formato incorreto, senhas fracas) e garantir que mensagens de erro apropriadas sejam exibidas. ✅
   - Fazer o login com novos usuarios criados e garantir que eles estejam com a role esperada. ✅

3. **Edição de Usuários Existentes:**
   - Selecionar um usuário existente e testar a funcionalidade de edição, alterando diferentes campos (nome, e-mail, papel, etc.) e verificar se as alterações são salvas corretamente. ⚠️
   - Testar a edição com dados inválidos e garantir que o sistema não permita a atualização e exiba mensagens de erro adequadas. ✅
   - Teste de exclusão de usuário. ✅

4. **Verificação de Persistência de Dados:**
   - Após a criação e edição de usuários, verificar se as informações persistem corretamente no banco de dados e são exibidas corretamente na tabela. ✅

5. **Testes de Usabilidade:**
   - Avaliar a interface da tabela para garantir que seja intuitiva e fácil de usar para administradores. ✅
   - Observar se as ações de criação e edição são realizadas de forma eficiente e sem confusões. ✅

6. **Testes de Responsividade:**
   - Testar a tabela de gerenciamento de usuários em diferentes tamanhos de tela (desktop, tablet, smartphone) para garantir que a interface se ajuste corretamente.
 ✅
   - Verificar se todos os elementos da tabela (botões, campos de entrada, etc.) são acessíveis e utilizáveis em dispositivos móveis. ✅
   - Avaliar se a funcionalidade de criação e edição de usuários é mantida em dispositivos com telas menores. ✅

---


# 🖼️ Imagens de Testes

## Tabela de gerenciamento de usuários

### Selecionar um usuário existente e testar a funcionalidade de edição, alterando diferentes campos (nome, e-mail, papel, etc.) e verificar se as alterações são salvas corretamente. ⚠️
- Ao tentar fazer a edição dos dados de um usuário já existente os campos de email e CPF estão bloqueados para alteração.

![image](/testes//assets/img%20edicao%20user.jpeg)
---
### Validado se novo usuário criado pela tabela de gerenciamento tem acesso ou não a funções de admin ✅

- Sem acesso as funções de admin - Usuário com role autenticado

![image](/testes//assets/opcoes%20novo%20user.jpeg)

- Com acesso as funções de admin - Usuário com role adminstrador

![image](/testes//assets/opcoes%20user%20admin.jpeg)

---

### Testes da tabela em diferentes tamanhos de telas ✅

- Desktop

![image](/testes/assets/desktop.png)

- Smartphone

![image](/testes//assets/phone.png)

- Tablet

![image](/testes//assets/tablet.png)

---
