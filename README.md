# Operació Nord Tec - Alicia Iamandi - 1A
> Documentació tècnica del projecte


# Índex

- [Enllaç](#enllaç)
- [Estat del projecte](#estat-del-projecte)
  - [Tasques realitzades](#tasques-realitzades)
- [Arquitectura de xarxa](#arquitectura-de-xarxa)
  - [Xarxes utilitzades](#xarxes-utilitzades)
  - [Interfície de la xarxa:](#interfície-de-la-xarxa)
- [Configuracions](#configuracions)
  - [Estructura de carpetes](#estructura-de-carpetes)
  - [Git i GitHub:](#git-i-github)
  - [Tallafoc amb iptables](#tallafoc-amb-iptables)
- [Incidències i solucions](#incidències-i-solucions)
  - [Incidència 1: Comanda no reconeguda al terminal](#incidència-1-comanda-no-reconeguda-al-terminal)
    - [Missatge d'error exacte](#missatge-derror-exacte)
    - [Quan](#quan)
    - [Causa](#causa)
    - [Solució](#solució)
  - [Decisions tècniques](#decisions-tècniques)
  - [Reflexions tècniques](#reflexions-tècniques)

## Enllaç

[GitHub](https://github.com/2627ali/README.md.git)

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

### Interfície de la xarxa:

- enp1s0: utilitzada per a la sortida del trànsit mitjançant NAT.
- enp3s0: utilitzada per aplicar la redirecció del trànsit HTTP.

## Configuracions

### Estructura de carpetes

El projecte està organitzat en diferents carpetes per separar els fitxers segons la seva funció:

- documentació.

- fitxers d'infraestructura.
- recursos del projecte.
- fitxers XML.
- fitxers YAML.

### Git i GitHub:

S'utilitza Git per controlar les versions dels fitxers i GitHub per allotjar el repositori remot.

> Taula de comandes

| Comanda         | Funció                                            |
| --------------- | -------------------------------------------------- |
| `git init`      | Crea un repositori Git nou.                        |
| `git status` | Mostra l'estat dels fitxers.               |
| `git add .`    | Afegeix els canvis per preparar-los per al commit.        |
| `git commit -m "missatge"`    | 

Desa els canvis en un commit.                |
| `git push`     | Puja els canvis del repositori local a GitHub. |
| `git pull`    | 

Actualitza el repositori local.                    |
| `git remote -v`      | Mostra els repositoris remots configurats.     |

### Tallafoc amb iptables

S'ha treballat amb el fitxer firewall.sh, que conté les regles per configurar el tallafoc mitjançant iptables.

Les configuracions treballades inclouen:

- Neteja de les regles anteriors.
- Configuració de les polítiques per defecte.
- Regles MASQUERADE per a les xarxes internes.
- Regla DNAT per redirigir el trànsit HTTP cap a 192.168.10.10.

**Per executar l'script:**

`sudo ./firewall.sh`


## Incidències i solucions

### Incidència 1: Comanda no reconeguda al terminal

#### Missatge d'error exacte

`bash: configuracio: command not found`

#### Quan

Durant una pràctica en què estava utilitzant el terminal integrat de Visual Studio Code.

#### Causa

Vaig escriure configuracio com si fos una comanda del terminal, però Bash no la reconeixia perquè no és una comanda vàlida.

#### Solució

Vaig revisar el missatge d'error, vaig tornar a la comanda anterior i vaig continuar executant les instruccions correctament.

### Decisions tècniques

1. **Organització per carpetes:** s'ha decidit separar els fitxers segons la seva funció per facilitar-ne la localització i mantenir l'ordre.

2. **Markdown:** s'ha escollit per documentar el projecte de manera clara i estructurada.

3. **Git:** s'utilitza per controlar les versions i guardar l'historial dels canvis.

4. **GitHub:** s'utilitza per tenir una còpia remota del projecte.

5. **Script firewall.sh:** s'ha utilitzat per agrupar les regles d'iptables en un únic fitxer i facilitar-ne l'execució.

### Reflexions tècniques

Aquest projecte m'està ajudant a familiaritzar-me amb diferents eines d'administració de sistemes i xarxes.

He après la importància de mantenir els fitxers organitzats i documentar els canvis que es fan durant les pràctiques.

També he entès que Git i GitHub permeten controlar les versions del projecte i mantenir un historial de les modificacions.

Finalment, he après que és important llegir els missatges d'error del terminal, identificar-ne la causa i comprovar que la solució aplicada funciona.

