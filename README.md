# PocketBudget

PWA de gestió de despeses personals, pensada per a iPhone i allotjament estàtic a GitHub Pages.

## Funcionalitats de la primera versió
- Dashboard amb saldo, ingressos i despeses del mes.
- Registre de moviments i historial filtrable.
- Categories i comptes personalitzables.
- Estadístiques mensuals per categoria.
- Emmagatzematge local amb IndexedDB.
- Exportació i importació de còpies JSON.
- Manifest PWA i Service Worker per a ús offline.
- Integració inicial amb Apple Dreceres mitjançant URL.

## Desenvolupament local
Obre el projecte amb un servidor estàtic (per exemple `python -m http.server 8000`) i visita `http://localhost:8000`. Service Workers i IndexedDB necessiten un context segur (`localhost` o HTTPS).

## Integració amb Dreceres
- Afegir despesa: `?action=add&type=expense&amount=4.50&category=food&description=Cafe`
- Afegir ingrés: `?action=add&type=income&amount=1200&category=salary&description=Nomina`
- Consultar saldo: `?action=balance`
- Consultar despeses del mes: `?action=month`

Les dades són locals i no s'envien a cap servidor. Es recomana exportar còpies de seguretat periòdiques.