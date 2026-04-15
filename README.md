###
ENTIDADES:

- Usuário
- Comunidade
- Recado
- Membership (relação usuário ↔ comunidade)

####
[ 👤 USUÁRIO ]
####
- CRIAÇÃO E AUTH:

 - [] Criar conta com: nome, email (único) e senha
 - [] Login com email e senha
 - [] Autenticação via JWT
 - [] (Opcional) Confirmação de conta por email


###
- PERFIL:
 - [] Editar nome
 - [] Adicionar/Editar avatar (URL ou upload — decidir)
 - [] Adicionar/Editar descrição (about)
       - Descrição inicia como null

Regras inciais:
 - [] Usuário só pode editar o próprio perfil
 - [] Email deve ser único


####
[ 💬 RECADOS ]
 - [] Recados são sempre privados
 - [] Apenas quem enviou ou recebeu pode visualizar

####

######
[👥 COMUNIDADE]
######
- FUNCIONALIDADES E CRIAÇÃO:
 - [] Usuário pode criar uma comunidade
       - Criador é automaticamente admin
       - Comunidade possui: admin | membro
 - [] Comunidade possui: nome, descrição, dono (admin)
 - [] Definir se a comunidade é pública ou privada
 - [] Usúario pode adicionar outros administradores
 - [] Qualquer membro pode criar um tópico
 - [] Membros podem deletar apenas o seus proprios tópicos
 - [] O Administrador pode deletar qualquer tópico/post
 - [] O Admnistrador pode expulsar um membro
 - [] Usuário pode solicitar entrada em comunidade
 - [] Usuário pode entrar diretamente (se pública)
 - [] Dono/admin pode aceitar ou recusar solicitações
 - []Usuário pode sair da comunidade


###
-REGRAS GENERICAS:
 - [] Apenas admin podeE: editar comunidade, aprovar membros
 - [] Usuário não pode entrar duas vezes na mesma comunidade


######
[🔗 MEMBERSHIP (Usuário ↔ Comunidade)] n:n
######
