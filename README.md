# DesafioUnimedBH_SQL
Repositório criado para os desafios do módulo de base de dados SQL e NOSQL

##**Desafio nº1 - E-commerce**

No desafio de E-commerce foi proposto que o cliente pudesse ser Pessoa Física (PF) ou pessoa jurídica (PJ), porém é um item exclusivo, ou seja não pode ser as duas opções. Quanto ao pagamento pode haver mais de uma forma cadastrada e quanto á entrega possui status e código de rastreio.

##**Desafio nº 2 - Sistema para oficina mecânica**

Foi proposto a estruturação de um sistema de controle e gerenciamento de execução de ordem de serviço em uma oficina.
•	Os tipos de serviços podem ser: Conserto ou Revisão;
•	Cada veículo é designado á uma equipe de mecânicos que identifica os serviços a serem executados, preenchem os com data de entrega e executam o serviço;
•	Uma OS pode conter vários serviços e os serviços podem estar em várias OS’s;

Foi pensado em uma tabela chamada OS, onde contém os seguintes relacionamentos:

Campo_Ligação_Tabela OS  |	Tabela 2	                |       Campo_Ligação	|   Tipo
Código_Serviço	         |Tabela_de_referência_de_MO	|Código_Serviço	      |Muitos para muitos
Código_Serviço	         |Tabela Serviço	            |Id Código_Serviço	  |Muitos para muitos
Tipo_de_Serviço	         |Tipo Serviço	              |Id Tipo_Serviço	    |Muitos para 1
Código_Cliente	         |Cliente	                    |Código_Cliente	      |Muitos para 1
Equipe	                 |Equipe	                    |Id Código_mecânico	  |Muitos para muitos
Código_Peças	           |Peças	                      |Id Codigo_Peças	    |Muitos para Muitos
