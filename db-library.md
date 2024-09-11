# DB University

//indviduo tutte le tabelle da inserire e definisco le caratteristiche

# table: dipartimenti
- id * PK UNSIGNED AI BIGINT
- Nome Dipartimento VARCHAR ()
- Tipi di Lauree VARCHAR ()
- Sbocchi professionali TEXT
- Corsi di Laurea UNSIGNED BIGINT (corsi_laurea_id)

# table: corsi_laurea
- id * PK UNSIGNED AI BIGINT
- Nome Corso di Laurea VARCHAR()
- Corsi Interni (corsi_interni_id)
- Studenti Iscritti BIGINT UNSIGNED (studenti_id)

# table: corsi_interni
- id* PK  UNSIGNED AI BIGINT
- Nome Corso VARCHAR()
- Durata Corso VARCHAR (60)
- Crediti Corso DECIMAL (2,0)
- Insegnante BIGINT UNSIGNED (insegnanti_id)
- Appelli BIGINT UNSIGNED (appelli_id)

# table: insegnanti
- id * PK UNSIGNED AI BIGINT
- Nome VARCHAR (80)
- Cognome VARCHAR(80)
- N. Telefono VARCHAR(14)
- Email VARCHAR(80)

# table: studenti
- id* PK UNSIGNED AI BIGINT
- Nome VARCHAR(80)
- Cognome VARCHAR(80)
- Codice Fiscale VARCHAR(16)
- Data di Nascita DATE
- N. Telefono VARCHAR(14)
- Email VARCHAR(80)

# table: appelli
- id* PK UNSIGNED AI BIGINT
- Tipo di Esame VARCHAR(20)
- Durata Esame VARCHAR(80)
- Date Appelli DATE
- Esiti Prove ? (esiti_id)

# table: esiti
- id* PK UNSIGNED AI BIGINT
- Data Esame DATE
- Studente Iscritto BIGINT UNSIGNED (studenti_id)
- Voto Esame DECIMAL (3,0)



