# DB University

//indviduo tutte le tabelle da inserire e definisco le caratteristiche

# universita_database
- id * PK AI BIGINT
- dipartimento (collegamento con tab dipartimenti) VARCHAR ()
- tipi di lauree in uscita VARCHAR ()
- studenti iscritti (collegamento con tab studenti) ?
- sbocchi professionali TEXT

# dipartimenti
- id * PK AI BIGINT
- nome dipartimento VARCHAR()
- corsi di laurea
- studenti iscritti ?

# corsi_di_laurea
- id * PK AI BIGINT
- nome corso di laurea VARCHAR()
- corsi interni (collegamento con tab corsi interni)
- studenti iscritti

# lista_corsi_interni
- id* PK AI BIGINT
- nome corso VARCHAR()
- durata corso VARCHAR (60)
- crediti corso DECIMAL (2,0)
- insegnante corso (collegamento con tab insegnanti) VARCHAR()
- date appelli DATE

# lista_insegnanti
- id * PK AI BIGINT
- nome VARCHAR (80)
- cognome VARCHAR(80)
- n. telefono VARCHAR(14)
- email VARCHAR(80)

# lista_studenti
- id* PK AI BIGINT
- nome VARCHAR(80)
- cognome VARCHAR(80)
- sesso VARCHAR(20)
- data di nascita DATE
- codice fiscale VARCHAR(16)
- n. telefono VARCHAR(14)
- email VARCHAR(80)



