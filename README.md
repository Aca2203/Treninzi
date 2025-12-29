# Treninzi
Aplikacija za praćenje treninga

# Model baze podataka
- Tabele:
	1. Sesija - sadrži podatke o datumu, početku, kraju i duzini trajanja treninga
	2. Vezba - sadrži naziv vežbe i tip opreme (telesna težina, mašina, tegovi,...)
	3. Sesija_vezba - trajno čuva podatke o tome koja vežba je bila urađena u kojoj sesiji
	4. Podaci_o_vezbi - generalizuje podatke o vežbi
	5. Podaci_snaga - specijalizacija podataka o vežbi koja čuva težinu (kg), broj serija i ponavljanja vežbe
	6. Podaci_kardio - specijalizacija podataka o vežbi koja čuva vreme trčanja, brzinu, nagib platforme,...
	7. Naziv_treninga - sadrži nazive treninga
	8. Trening_vezba - čuva podatke o tome koja vežba pripada kom tipu treninga
	
- Veze (Tabela1 (kardinalnost1) -> Tabela2 (kardinalnost2)):
	- 