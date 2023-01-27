# twitter_clone-mvc
 
create database twiter_clone

create table usuarios(
	id  INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
	nome varchar(100) not null,
	email varchar(150) not null,
	senha varchar(32) not null
	

);
create table tweets(
	id  INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
	id_usuarios int not null,
	tweet varchar(140) not null,
	data datetime default current_timestamp
	

);

create table usuarios_seguidores(
	id  INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
	id_usuario int not null,
	id_usuario_seguindo int not null
	

);
