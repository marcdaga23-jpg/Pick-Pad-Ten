# 🏆 Torneig Triatló Raqueta (Tennis · Pàdel · Pickleball)

Aplicació web lleugera (sense servidor ni dependències externes) preparada per allotjar-se gratuïtament a **GitHub Pages** i gestionar el torneig de **14 parelles**.

## 📋 Característiques principals
- **Lligueta de 14 parelles (42 partits):** Control automàtic perquè cada parella jugui exactament **2 partits de Tennis, 2 de Pàdel i 2 de Pickleball**.
- **Sorteig en directe:** Generador aleatori de parella perquè esculli pista, esport i rival al moment.
- **Sistema de puntuació oficial:** 3 punts per victòria, 1 punt per derrota i resolució d'empats als 15 minuts mitjançant **Punt d'Or**.
- **Classificació automàtica:** Ordenació en temps real per punts totals, diferència de punts/jocs i victòries.
- **Fase Final d'Or i Plata:**
  - **1r al 8è:** Quarts de final, Semifinals i Final d'Or.
  - **9è i 10è:** Passen directament a Semifinals de Plata.
  - **11è al 14è:** Juguen Quarts de final de Plata.

## 🚀 Com publicar-ho a GitHub Pages en 2 minuts
1. Crea un repositori nou a [GitHub](https://github.com) (per exemple: `torneig-raqueta`).
2. Puja els fitxers `index.html` i `README.md` d'aquest paquet al repositori.
3. Ves a **Settings → Pages** dins del repositori.
4. A **Source**, selecciona la branca `main` i la carpeta `/ (root)`, i fes clic a **Save**.
5. En menys d'un minut tindràs la teva URL pública (`https://el-teu-usuari.github.io/torneig-raqueta/`) per compartir o convertir en codi QR.

## 🔐 Accés Organitzador
- **PIN per defecte:** `1234` (pots modificar-lo editant la línia `const ADMIN_PIN = "1234";` dins de `index.html`).
- *Nota sobre dades en temps real:* Aquesta versió guarda les dades al navegador (`localStorage`) i permet exportar/importar un fitxer `.json`. Si vols que múltiples mòbils vegin els canvis instantàniament des d'un sol dispositiu de taula de control, només cal connectar l'objecte `state` a una base de dades gratuïta com **Firebase Realtime Database** o **Supabase**.
