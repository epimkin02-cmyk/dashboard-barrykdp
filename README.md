# Barry KDP – Webinar Tracking (Prototyp)

Interner Dashboard-Prototyp im Barry-KDP-CI. Enthält nur **Beispieldaten** und einen **Demo-Login ohne echte Zugangskontrolle** – bitte noch nicht mit echten Zahlen befüllen.

## In 5 Minuten online (GitHub Pages)

1. Neues Repository auf GitHub anlegen (z. B. `barry-dashboard`), am besten **privat**? → Achtung: GitHub Pages aus privaten Repos gibt es nur mit GitHub Pro/Team. Im Free-Plan muss das Repo **public** sein – für diesen Prototyp mit Beispieldaten okay.
2. Diese Dateien ins Repo hochladen (`index.html`, `.nojekyll`, `README.md`).
3. Im Repo: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / root → Save.**
4. Nach 1–2 Minuten ist das Dashboard erreichbar unter:
   `https://<dein-account>.github.io/barry-dashboard/`

## Eigene Subdomain (empfohlen)

Statt der GitHub-URL: `dashboard.thepublishermethod.com`

1. In **Settings → Pages → Custom domain** eintragen: `dashboard.thepublishermethod.com`
2. Beim DNS-Anbieter der Domain einen **CNAME-Record** anlegen:
   `dashboard` → `<dein-account>.github.io`
3. „Enforce HTTPS“ aktivieren, sobald das Zertifikat da ist (dauert ein paar Minuten).

Die Hauptseite thepublishermethod.com bleibt davon komplett unberührt.

## Wichtig: Sicherheit

- GitHub Pages kann **keinen Passwortschutz** – der Demo-Login in der Seite ist nur Optik.
- Deshalb: Prototyp nur mit Beispieldaten betreiben und den Link nur intern teilen.
- Die **echte Version** (mit echten Zahlen aus Make/GHL/Stripe) gehört hinter einen echten Login –
  z. B. Softr (No-Code) oder Vercel/Netlify + Supabase Auth. Siehe Konzept-Dokument.
