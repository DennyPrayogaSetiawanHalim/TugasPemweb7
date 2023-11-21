# TugasPemweb7

Command SQL untuk tugas :

CREATE DATABASE tugasPemweb;
USE tugasPemweb;

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";

CREATE TABLE mahasiswa (
  nim bigint(10) NOT NULL,
  nama varchar(50) NOT NULL,
  prodi varchar(50) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

ALTER TABLE mahasiswa
  ADD PRIMARY KEY (nim);

INSERT INTO mahasiswa (nama, nim, prodi)
VALUES ('Bobi', 2012001, 'Teknik Informatika'),
('Tobi', 2012002, 'Teknik Informatika'),
('Robi', 2013004, 'Teknik Elektro'),
('Roni', 2014005, 'Teknik Telekomunikasi'),
('Toni', 2015001, 'Sains Data'),
('Doni', 2016001, 'Teknik Sipil');

COMMIT;


