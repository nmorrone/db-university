# DB University

//indviduo tutte le tabelle da inserire e definisco le caratteristiche

# table: dipartimenti
- id * PK AI BIGINT
- Nome Dipartimento (collegamento con tab dipartimenti) VARCHAR ()
- Tipi di Lauree VARCHAR ()
- Sbocchi professionali TEXT
- Corsi di Laurea BIGINT

# table: corsi_laurea
- id * PK AI BIGINT
- Nome Corso di Laurea VARCHAR()
- Corsi Interni
- Studenti Iscritti BIGINT

# table: corsi_interni
- id* PK AI BIGINT
- Nome Corso VARCHAR()
- Durata Corso VARCHAR (60)
- Crediti Corso DECIMAL (2,0)
- Insegnante BIGINT
- Appelli BIGINT

# table: insegnanti
- id * PK AI BIGINT
- Nome VARCHAR (80)
- Cognome VARCHAR(80)
- N. Telefono VARCHAR(14)
- Email VARCHAR(80)

# table: studenti
- id* PK AI BIGINT
- Nome VARCHAR(80)
- Cognome VARCHAR(80)
- Codice Fiscale VARCHAR(16)
- Data di Nascita DATE
- N. Telefono VARCHAR(14)
- Email VARCHAR(80)

# table: appelli
- id* PK AI BIGINT
- Tipo di Esame VARCHAR(20)
- Durata Esame VARCHAR(80)
- Date Appelli DATE
- Esiti Prove ?

# table: esiti
- id* PK AI BIGINT
- Data Esame DATE
- Studente Iscritto BIGINT
- Voto Esame DECIMAL (3,0)



