# 🔥 Loop Trauma — Escape Room 3D

> Un escape room en realitat virtual desenvolupat amb **A-Frame / WebVR**  
> Inspirat en l'univers de Dark Souls · Narrativa psicològica · Bullet Hell final

---

## 🔗 Links del Projecte

| Recurs | Enllaç |
|--------|--------|
| 📄 Documentació (Google Drive) | [Veure document](https://docs.google.com/document/d/1nniBZNZ_fGzI72PQ6o1iP-KDDM5hicbERVUFDCEpypw/edit?usp=sharing) |
| 📊 Planificació temporal (Excel) | _Afegir URL de l'Excel aquí_ |
| 🎮 Jugar ara (pàgina d'inici) | [Iniciar el joc](https://caldopollo66.github.io/LoopTraumaEscaperoom/intro.html) |

---

## 📖 Descripció

**Loop Trauma** és un escape room en 3D on el jugador es troba atrapat en un cicle de trauma inspirat en l'estètica i narrativa de Dark Souls. Ha de resoldre preguntes, recollir objectes i enfrontar-se a un jefe final en un combat de bullet hell per trencar el bucle i escapar.

El joc utilitza **A-Frame 1.4–1.5** per renderitzar escenes WebVR que funcionen directament al navegador, sense instal·lació.

---

## 🗺️ Estructura del Joc

```
intro.html
    └── menu.html
            └── anor_londo.html   ← Escena principal
                    └── sala_jefe.html   ← Combat final (Bullet Hell)
```

### Escenes

| Arxiu | Escena | Estat |
|-------|--------|-------|
| `intro.html` | Portada / Pantalla inicial | ✅ Completat |
| `menu.html` | Menú principal | ✅ Completat |
| `anor_londo.html` | Anor Londo — escena principal | ✅ Completat |
| `sala_jefe.html` | Arena del jefe final (Bullet Hell) | ✅ Completat |
| `Bosque.html` | Bosc místic | 🔄 En desenvolupament |

---

## 🎮 Com Jugar

### Controls
- **WASD** — Moure's per l'escena
- **Ratolí** — Mirar al voltant (look-controls)
- **Cursor vermell** — Apuntar a objectes clickables
- **Clic** — Interactuar amb objectes

### Flux de joc a Anor Londo

1. **Clica Artorias** → Respon la pregunta sobre Dark Souls → Apareix la **Sword**
2. **Clica el Caballero** → Respon la pregunta sobre Dark Souls → Apareix l'**Estus Flask**
3. **Clica el Càliz** directament → S'afegeix a l'inventari
4. Amb els **3 objectes** → Clica l'**Altar** → Es fa de nit, apareix el Boss, sona el diàleg
5. Quan **acaba el diàleg** → La **Porta** s'obre
6. **Clica la Porta** → Entres a la **Sala del Jefe**

### Sala del Jefe — Bullet Hell
- Esquiva **5 patrons d'atac** del boss
- Tens **3 vides** (cors)
- El boss canvia de fase cada 4 segons

---

## 🧩 Objectes del Joc

| Objecte | Com obtenir-lo |
|---------|---------------|
| 🏆 **Càliz** | Clic directe sobre el model |
| ⚔️ **Sword** | Respondre correctament el quiz d'Artorias |
| 🧪 **Estus Flask** | Respondre correctament el quiz del Caballero |

### Preguntes / Proves

**Quiz 1 — Artorias:**
> Quin és el nom del monarca de la flama en Dark Souls?  
> A) Filianore · **B) Gwyn** · C) Gwyndolin · D) Gwynevere

**Quiz 2 — Caballero:**
> Quin és el nom de la donzella de la llum de la lluna?  
> A) Ornstein · B) Gwynevere · **C) Gwyndolin** · D) Anri of Astora

---

## 📁 Estructura del Repositori

```
LoopTraumaEscaperoom/
├── intro.html              # Pantalla d'inici
├── menu.html               # Menú principal
├── anor_londo.html         # Escena principal
├── sala_jefe.html          # Arena del jefe (Bullet Hell)
├── Bosque.html             # Bosc místic (WIP)
├── probas.html             # Proves de desenvolupament
├── probas2.html            # Proves de desenvolupament
├── test.html               # Sandbox de test
├── modelos/                # Models 3D (.glb)
│   ├── anor_londo.glb
│   ├── londo_exterior.glb
│   ├── boos.glb
│   ├── knight_artorias.glb
│   ├── knight.glb
│   ├── door.glb
│   ├── altar.glb
│   ├── caliz.glb
│   ├── sword.glb
│   ├── estus.glb
│   └── virtue.glb
├── musica/                 # Àudio
│   ├── DS3.mp3
│   └── Dialogo.mp3
├── IMG/                    # Imatges i textures
│   ├── lonod.jpg
│   └── banana.png
└── assets/                 # Altres recursos
```

---

## 🛠️ Tecnologies

| Tecnologia | Versió | Ús |
|------------|--------|----|
| [A-Frame](https://aframe.io) | 1.4.2 / 1.5.0 | Motor WebVR / 3D |
| HTML5 | — | Estructura i lògica |
| JavaScript (Vanilla) | ES6+ | Components A-Frame, lògica de joc |
| Three.js | (inclòs a A-Frame) | Detecció de col·lisions, vectors 3D |
| CSS3 | — | HUD, overlays, efectes |

---

## 👥 Equip

Projecte desenvolupat com a treball de curs de Realitat Virtual.

| Membre | Rol |
|--------|-----|
| Membre 1 | Programador principal · A-Frame · Lògica de joc |
| Membre 2 | Dissenyador 3D · Assets · Posicionament d'escenes |
| Membre 3 | Disseny narratiu · Preguntes · Història |

---

## 📋 Llicència

Projecte educatiu. Els models 3D i la música poden estar subjectes a drets de tercers.

---

<div align="center">

**Loop Trauma** · Escape Room 3D · 2024–2025  
Fet amb ❤️ i A-Frame

[🎮 Jugar ara](https://caldopollo66.github.io/LoopTraumaEscaperoom/intro.html) · [📄 Documentació](https://docs.google.com/document/d/1nniBZNZ_fGzI72PQ6o1iP-KDDM5hicbERVUFDCEpypw/edit?usp=sharing) · [🐙 GitHub](https://github.com/Caldopollo66/LoopTraumaEscaperoom)

</div>
