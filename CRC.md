# CRC de classes baseado em histórias de usuário


User Story: Como usuário iniciante, quero criar uma conta e fazer login para acessar meus progressos e conquistas.
User Story: Como usuário, quero ter acesso a uma primeira lição de programação com perguntas simples para começar a aprender.
User Story: Como usuário, quero ganhar pontos a cada exercício resolvido para acompanhar meu progresso e me sentir motivado.
---

| Classe           | Responsabilidade                                                                                                                                                                                                                       | Contribuição                                                 |
|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------|
| Usuário          | - Saber seu nome e credenciais de acesso<br> - Saber quais certificados recebeu<br> - Saber quais trilhas estão em andamento<br> - Saber quais trilhas foram concluídas<br> - Receber Conquistas ao completar desafios<br>             | - Conquitas<br> - ProgressoUsuario<br>                       |
| Conquistas       | - Conhecer o progresso do usuário<br> - Gerar conquista para o usuário<br> - Saber seus requisitos para ser adquirida<br>                                                                                                              | - Usuario<br> - ProgressoUsuario                             |
| Lições           | - Representar um exercício<br> - Ter um enunciado<br> - Ter alternativas e resposta(s)<br> - Validar respostas do usuário<br> - Oferecer explicação sobre a questão<br> - Cadastrar progresso do usuário<br> - Fornecer pontuação <br> | - ProgressoUsuario<br> - Trilhas                             |
| Trilha           | - Saber seu nome e tema <br> - Organizar sequência de exercícios<br> - Cadastrar progresso do usuário <br> - Gerar certificado ao ser concluída<br> - Associa o nome do usuário<br>                                                    | - ProgressoUsuario<br> - Lições                              |
| ProgressoUsuario | - Verifica se alguma conquista foi obtida<br> - Registra progresso da trilha<br> - Registra pontuação das questões<br> - Vincula usuário com Trilha<br>                                                                                | - Trilha <br> - Lições <br> - Conquistas <br> - Usuário <br> |
