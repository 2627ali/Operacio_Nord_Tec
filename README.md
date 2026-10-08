# Operació Nord Tec - Alicia Iamandi - 1A
## Índex

- Estat del projecte 
- Arquitectura de xarxa
- Configuracions 
- Incidències i solucions
  - Missatge d'error exacte
  - Quan
  - Causa
  - Solució
  - Detectada per...
  - Decisions tècniques
  - Reflexions tècniques
  
## Llista ordenada
### Passos per pujar un canvi a GitHub

1. Fer els canvis necessaris als fitxers.
2. Comprovar els canvis amb `git status`.
3. Afegir els fitxers amb `git add .`.
4. Fer un commit amb `git commit -m "Nou intent"`.
5. Pujar els canvis a GitHub amb `git push -u origin main`.

## Llista de tasques

- [ ] Crear el repositori
- [ ] Fer canvis al README.md
- [ ] Fer el commit dels canvis
- [ ] Pujar els canvis a GitHub

## Enllaç

[GitHub](https://github.com/2627ali/README.md.git)

## Bloc de codi

```
git init
git --version
git status
git branch
git commit -m ""
git remote add origin
git push -u origin main
git add .
git commit -m "Nou intent"
git push -u origin main 
```

## Taula de comandes

| Comanda         | Què fa?                                            |
| --------------- | -------------------------------------------------- |
| `git init`      | Crea un repositori Git nou.                        |
| `git --version` | Mostra la versió de Git instal·lada.               |
| `git status`    | Mostra l'estat dels fitxers del repositori.        |
| `git branch`    | Mostra les branques del repositori.                |
| `git add .`     | Afegeix els canvis per preparar-los per al commit. |
| `git commit`    | Guarda els canvis en un commit.                    |
| `git push`      | Puja els canvis del repositori local a GitHub.     |

## Incidències 

### Què va passar?

Quan estava treballant amb el terminal de VS Code, vaig escriure una comanda incorrectament i em va aparèixer el missatge `bash: configuracio: command not found`.

### Per què?

Va passar perquè vaig escriure `configuracio` com si fos una comanda, però aquesta comanda no existeix i Bash no la va poder reconèixer.

### Com s'ha resolt?

Vaig comprovar l'error que m'indicava el terminal i vaig tornar a la comanda anterior. Després vaig continuar escrivint les comandes correctament i vaig poder seguir amb la pràctica.