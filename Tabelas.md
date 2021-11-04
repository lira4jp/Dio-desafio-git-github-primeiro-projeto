Desafio para criar tabelas para o desafio gerenciador de espaço naves do Star Wars. 



CREATE TABLE Planetas
(
IdPlaneta int NOT NULL,
Nome varchar(50) NOT NULL,
Rotacao float NOT NULL,
Orbita float NOT NULL,
Diametro float NOT NULL,
Clima varchar(50) NOT NULL,
Populacao int NOT NULL,
)

CREATE TABLE Naves
(
IdNave int NOT NULL,
Nome varchar(100) NOT NULL,
Modelo varchar(150) NOT NULL,
Passageiros int NOT NULL,
Carga float NOT NULL,
Classe varchar(100) NOT NULL,
)

CREATE TABLE Pilotos
(
IdPiloto int NOT NULL,
Nome varchar(200) NOT NULL,
AnoNascimento varchar(10) NOT NULL,
IdPlaneta int NOT NULL,
)

CREATE TABLE PilotosNaves
(
IdPiloto int NOT NULL,
IdNave int NOT NULL,
FlagAutorizado bit NOT NULL,
)

CREATE TABLE HistoricoViagens
(
IdNave int NOT NULL,
IdPiloto int NOT NULL,
DtSaida datetime NOT NULL,
DtChegada datetime NULL
)