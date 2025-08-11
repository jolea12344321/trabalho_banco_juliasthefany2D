## trabalho_banco_juliasthefany2D

Clínica Médica Online
Tema do Projeto
Banco de dados para gestão de clínica médica, organizando informações de pacientes, médicos, consultas, especialidades e prontuários.

Descrição do Problema
Controlar agendas, registros de pacientes, atendimentos e informações médicas de forma centralizada e segura, evitando redundância e garantindo integridade dos dados.
Particularmente tive problemas com o MySQL Workbench ao testar as queries, mas consegui resolver.

Entidades e Relacionamentos
Especialidade: Lista as especialidades médicas (ex: Cardiologia, Pediatria, Ortopedia).

Médico: Informações sobre o profissional, vinculado a uma especialidade.

Paciente: Dados cadastrais e contato dos pacientes.

Consulta: Registro da consulta realizada, incluindo data, horário, médico e paciente.

Prontuario: Histórico médico do paciente, vinculado a consultas específicas.

As tabelas são relacionadas com chaves estrangeiras, garantindo integridade referencial.

Estrutura do Projeto
/model: diagramas e documentação da modelagem

/sql: scripts SQL para criar tabelas, inserir dados, consultas e índices

/docs: documentação da normalização até a 3FN

/screenshots: capturas de tela do MySQL Workbench

README.md: este arquivo

Tecnologias Usadas
MySQL Workbench

dbdiagram.io (para modelagem)

SQL (DDL, DML)

Prints e Exemplos das Consultas

ex: JOIN Paciente p ON c.PacienteID = p.PacienteID
JOIN Medico m ON c.MedicoID = m.MedicoID
WHERE c.DataConsulta BETWEEN NOW() AND DATE_ADD(NOW(), INTERVAL 7 DAY)
AND c.Status = 'Agendada'
ORDER BY c.DataConsulta ASC;

<img width="1007" height="413" alt="Captura de tela 2025-08-11 002819" src="https://github.com/user-attachments/assets/27f39462-68d0-4d1c-865a-e71bb33a4028" /> 
## Autora 
Julia Sthefany 2D (N20) julia.santos.assis@escola.pr.gov.br

