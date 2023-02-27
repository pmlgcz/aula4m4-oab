# aula4m4-oab


use escritorio;
CREATE TABLE `advogado` (
  `oab` int(30) NOT NULL primary key auto_increment,
  `nome` varchar(60) DEFAULT NULL,
  `endereco` varchar(60) DEFAULT NULL,
  `codarea` int(30) NOT NULL
);

CREATE TABLE `area_atuacao` (
`codarea` int(11) NOT NULL,
`descricao` varchar(30) DEFAULT NULL
);

CREATE TABLE `cliente` (
`codcliente` int(11) NOT NULL,
`nome` varchar(30) DEFAULT NULL,
`endereco` varchar(60) DEFAULT NULL
);

CREATE TABLE `causa` (
`codcausa` int(11) NOT NULL,
`dataabertura` date,
`descricao` varchar(30) DEFAULT NULL,
`dataencerramento` date,
`codarea` int(11),
`oab` int(30)
);
