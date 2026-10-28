# Montørplan

Prototype for planlegging av montører. Jobbene ligger i en kø per montør, og datoene beregnes ut fra rekkefølge og varighet. Når én jobb forsinkes eller en hastejobb legges inn, planlegges resten automatisk om.

**Prototype med eksempeldata.** Ingenting lagres, og ingen SMS sendes.

## Funksjoner

- Tidslinje for Q1 2027 med helger og påskehelligdager
- Tre jobbtyper: låst dato, kundevindu og fleksibel
- Forleng jobber, endre rekkefølge, sett tidligste startdato og flytt jobber mellom montører
- Hastejobber som legges først i køen
- Filtrering på jobbtype og status
- Kontrollpunkt: alle endringer er et utkast til de er sett over og godkjent
- Oversikt over hvilke kunder som får SMS og hvilke som må følges opp manuelt

## Kjøre lokalt

Åpne `index.html` i en nettleser. Det trengs ingen installasjon eller byggesteg.

## Publisere

Repoet kan kobles direkte til Cloudflare Pages:

- Build command: (tom)
- Output directory: `/`

For innlogging foran demoen kan Cloudflare Access (Zero Trust) slås på for adressen.

## Videre arbeid

- Database og innlogging (Supabase, EU-region)
- SMS-varsler med svar fra kunder
- Synk til Google Kalender
- Mobilvisning for montører
- Endringslogg
