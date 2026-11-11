# Operació Nord Tec - Alicia Iamandi - 1A
> Documentació tècnica del projecte


# Índex

- [Estat del projecte](#estat-del-projecte)
  - [Tasques realitzades](#tasques-realitzades)
- [Arquitectura de xarxa](#arquitectura-de-xarxa)
  - [Xarxes utilitzades](#xarxes-utilitzades)
- [Configuracions](#configuracions)
- [Incidències i solucions](#incidències-i-solucions)
  - [Missatge d'error exacte](#missatge-derror-exacte)
  - [Quan](#quan)
  - [Causa](#causa)
  - [Solució](#solució)
  - [Detectada per...](#detectada-per)
  - [Decisions tècniques](#decisions-tècniques)
  - [Reflexions tècniques](#reflexions-tècniques)
- [Llista ordenada](#llista-ordenada)
  - [Passos per pujar un canvi a GitHub](#passos-per-pujar-un-canvi-a-github)
- [Llista de tasques](#llista-de-tasques)
- [Enllaç](#enllaç)
- [Bloc de codi](#bloc-de-codi)
- [Taula de comandes](#taula-de-comandes)
- [Incidències](#incidències)
  - [Què va passar?](#què-va-passar)
  - [Per què?](#per-què)
  - [Com s'ha resolt?](#com-sha-resolt)

## Estat del projecte

El projecte Operació NordTec consisteix a realitzar diferents pràctiques relacionades amb la configuració, l'administració i la seguretat de sistemes i xarxes.

Per organitzar i documentar el projecte, s'utilitzen eines com Visual Studio Code, Git i GitHub.

### Tasques realitzades

- Creació de l'estructura inicial de carpetes del projecte.
- Instal·lació de Visual Studio Code.
- Instal·lació de les extensions Markdown All in One, Markdown Preview Enhanced i Material Icon Theme
- Instal·lació de Git i comprovació de la seva versió.
- Creació del fitxer README.md.
- Creació i configuració del repositori Git.
- Connexió del repositori local amb GitHub.
- Pràctica de les comandes bàsiques de Git.
- Documentació de les pràctiques utilitzant Markdown.
- Treball amb un script de configuració del tallafoc mitjançant iptables.

## Arquitectura de xarxa

En les pràctiques s'han treballat diferents xarxes i interfícies per configurar el tallafoc i gestionar el trànsit de xarxa.

### Xarxes utilitzades

| Xarxa         | Adreça IP                                            |
| --------------- | -------------------------------------------------- |
| Xarxa 1      | 192.168.10.0/24                        |
| Xarxa 2 | 192.168.20.0/24               |
| Xarxa 3    | 10.0.0.0/24        |

## Configuracions

Aquí explicaré les configuracions realitzades.

> [!NOTE]
> **Sugeriment**
> 
> Abans de modificar una configuració, comprova primer l'estat actual del sistema.

## Incidències i solucions

> [!WARNING]
> **Avís**
>
> Abans d'aplicar una solució, és important identificar correctament la causa de l'error.

> [!NOTE]
> **Recordatori**
>
> Una vegada solucionada la incidència, cal comprovar que el problema no torni a aparèixer.

### Missatge d'error exacte

Aquí escriuré el missatge d'error.

### Quan

Aquí explicaré quan va passar.

### Causa

Aquí explicaré la causa de l'error.

### Solució

Aquí explicaré com es va solucionar.

### Detectada per...

Aquí indicaré qui va detectar la incidència.

### Decisions tècniques

Aquí explicaré les decisions tècniques preses.

> [!IMPORTANT]
> **Decisió**
>
> S'ha decidit utilitzar aquesta configuració perquè ...

### Reflexions tècniques

Aquí explicaré les reflexions sobre el problema.

> [!NOTE]
> **Aprenentatge**
>
> Aquesta incidència m'ha ajudat a entendre que ...

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