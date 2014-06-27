create table pessoa (
id int not null primary key identity,
nome varchar(200) not null,
rg varchar(30) not null, -- fazer trigger para permitir 'NAO INFORMADO'
cpf varchar(30) not null
)

create index pessoa_id on pessoa (id)

create table usuarios (
id int not null primary key identity,
id_pessoa int not null foreign key references pessoa(id),
usr varchar(100) not null,
pwd varchar(100) not null,
)

create table sys_parameters (
id int not null primary key identity,
descricao varchar(200) not null,
grupo varchar not null,
tipo varchar(1) not null check (tipo in ('B', 'S', 'F', 'I', 'D')),
valor varchar null
)


