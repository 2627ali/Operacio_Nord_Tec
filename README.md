# Operació Nord Tec - Alicia Iamandi - 1A
> Documentació tècnica del projecte


# Índex

- [1. Estat del projecte](#1-estat-del-projecte)
  - [1.1 Tasques realitzades](#11-tasques-realitzades)
- [2. Arquitectura de xarxa](#2-arquitectura-de-xarxa)
  - [2.1 Xarxes utilitzades](#21-xarxes-utilitzades)
  - [2.2 Interfície de la xarxa:](#22-interfície-de-la-xarxa)
  - [2.3 Esquema de xarxa](#23-esquema-de-xarxa)
- [3. Configuracions](#3-configuracions)
  - [3.1 Estructura de carpetes](#31-estructura-de-carpetes)
  - [3.2 Git i GitHub:](#32-git-i-github)
  - [3.3 Tallafoc amb iptables](#33-tallafoc-amb-iptables)
- [4. Incidències i solucions](#4-incidències-i-solucions)
  - [4.1 Incidència 1: Comanda no reconeguda al terminal](#41-incidència-1-comanda-no-reconeguda-al-terminal)
    - [4.1.1 Missatge d'error exacte](#411-missatge-derror-exacte)
    - [4.1.2 Quan](#412-quan)
    - [4.1.3 Causa](#413-causa)
    - [4.1.4 Solució](#414-solució)
    - [4.1.5 Detectada per:](#415-detectada-per)
  - [4.2 Decisions tècniques](#42-decisions-tècniques)
  - [4.3 Reflexions tècniques](#43-reflexions-tècniques)

## 1. Estat del projecte

El projecte Operació NordTec consisteix a realitzar diferents pràctiques relacionades amb la configuració, l'administració i la seguretat de sistemes i xarxes.

Per organitzar i documentar el projecte, s'utilitzen eines com Visual Studio Code, Git i GitHub.

### 1.1 Tasques realitzades

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

## 2. Arquitectura de xarxa

En les pràctiques s'han treballat diferents xarxes i interfícies per configurar el tallafoc i gestionar el trànsit de xarxa.

### 2.1 Xarxes utilitzades

| Xarxa         | Adreça IP                                            |
| --------------- | -------------------------------------------------- |
| Xarxa 1      | 192.168.10.0/24                        |
| Xarxa 2 | 192.168.20.0/24               |
| Xarxa 3    | 10.0.0.0/24        |

### 2.2 Interfície de la xarxa:

- *enp1s0:* utilitzada per a la sortida del trànsit mitjançant NAT.
- *enp3s0*: utilitzada per aplicar la redirecció del trànsit HTTP.

### 2.3 Esquema de xarxa


## 3. Configuracions

### 3.1 Estructura de carpetes

El projecte està organitzat en diferents carpetes per separar els fitxers segons la seva funció:

- documentació.
- fitxers d'infraestructura.
- recursos del projecte.
- fitxers XML.
- fitxers YAML.

### 3.2 Git i GitHub:

S'utilitza Git per controlar les versions dels fitxers i GitHub per allotjar el repositori remot. Això permet guardar els canvis, consultar l'historial i mantenir una còpia del projecte en línia.

**Taula de comandes**

| Comanda         | Funció                                            |
| --------------- | -------------------------------------------------- |
| `git init`      | Crea un repositori Git nou.                        |
| `git status` | Mostra l'estat dels fitxers.               |
| `git add .`    | Afegeix els canvis per preparar-los per al commit.        |
| `git commit -m "missatge"`    | Desa els canvis en un commit.                |
| `git push`     | Puja els canvis del repositori local a GitHub. |
| `git pull`    | Actualitza el repositori local.                    |
| `git remote -v`      | Mostra els repositoris remots configurats.     |

### 3.3 Tallafoc amb iptables

S'ha treballat amb el fitxer firewall.sh, que conté les regles per configurar el tallafoc mitjançant iptables.

Les configuracions treballades inclouen:

- Neteja de les regles anteriors.
- Configuració de les polítiques per defecte.
- Regles MASQUERADE per a les xarxes internes.
- Regla DNAT per redirigir el trànsit HTTP cap a 192.168.10.10.

**Per executar l'script:**

`sudo ./firewall.sh`


## 4. Incidències i solucions

### 4.1 Incidència 1: Comanda no reconeguda al terminal

#### 4.1.1 Missatge d'error exacte

`bash: configuracio: command not found`

#### 4.1.2 Quan

Durant una pràctica en què estava utilitzant el terminal integrat de Visual Studio Code.

#### 4.1.3 Causa

Vaig escriure configuracio com si fos una comanda del terminal, però Bash no la reconeixia perquè no és una comanda vàlida.

#### 4.1.4 Solució

Vaig revisar el missatge d'error, vaig tornar a la comanda anterior i vaig continuar executant les instruccions correctament.

#### 4.1.5 Detectada per:

@AliciaIamandi

### 4.2 Decisions tècniques

1. **Organització per carpetes:** s'ha escollit separar els fitxers segons la seva funció per facilitar-ne la localització i mantenir el projecte ordenat. Una alternativa hauria estat guardar tots els fitxers en una mateixa carpeta, però seria més difícil trobar-los.
2. **Markdown:** s'ha escollit aquest format perquè permet crear documentació clara i estructurada. Una alternativa hauria estat utilitzar un document de text o un processador de textos.
3. **Git:** s'ha escollit per controlar les versions i guardar un historial dels canvis. Una alternativa hauria estat guardar diferents còpies dels fitxers manualment.
4. **GitHub:** s'ha escollit per allotjar el repositori remot i tenir una còpia del projecte en línia. Una alternativa hauria estat mantenir únicament el repositori local.
5. **Script firewall.sh:** s'ha escollit agrupar les regles d'iptables en un únic fitxer per facilitar-ne l'execució i la gestió. Una alternativa hauria estat introduir les regles manualment al terminal una per una.

### 4.3 Reflexions tècniques

Aquest projecte m'està ajudant a familiaritzar-me amb diferents eines d'administració de sistemes i xarxes.

He après la importància de mantenir els fitxers organitzats i documentar els canvis que es fan durant les pràctiques.

També he entès que Git i GitHub permeten controlar les versions del projecte i mantenir un historial de les modificacions.

Finalment, he après que és important llegir els missatges d'error del terminal, identificar-ne la causa i comprovar que la solució aplicada funciona.
