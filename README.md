# Proiect MAP - Gestiune de inventar

Proiect individual la disciplina Metode avansate de programare, anul universitar 2026-2027.

## Autor

- **Nume:** Serfezi Eduard 
- **Grupa:** 2.2
- **Marca:** 615708
- **Tema:** Tema numarul 4 - Gestiune de inventar

## Descriere

Aplicatia de gestiune a inventarului este un sistem digital care centralizeaza evidenta produselor, permitand monitorizarea rapida a stocurilor, a preturilor si a miscarilor de marfa. Aceasta rezolva problema organizarii haotice si a erorilor umane frecvente in evidentele manuale, prevenind situatiile in care ramai brusc fara produse importante sau blochezi bani in stocuri inutile.

## Tehnologii

Python 3.13 cu Flask

## Rulare

```
docker build -t map-proiect .
docker run -d -p 8080:8080 map-proiect
```

Aplicatia asculta pe portul 8080. Verificati:

```
curl http://localhost:8080/health
curl http://localhost:8080/version
```

## Testare

```
pip install -r requirements.txt pytest pytest-cov
python -m pytest --cov=src
```

## Rutele implementate

| Ruta | Metoda | Descriere |
|---|---|---|
| `/health` | GET | Starea serviciului |
| `/version` | GET | Versiunea si commit-ul din care a fost construita imaginea |
| `/` | GET | Pagina de prezentare |
| `/reset` | POST | Goleste datele din memorie |
| [ruta temei] | [metoda] | [descriere] |

## Decizii de implementare

**
