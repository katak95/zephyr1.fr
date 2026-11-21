# zephyr1.fr

Site vitrine statique de Zephyr1 (HTML/CSS/JS, sans build).

## Aperçu local
```bash
python3 -m http.server 8765
```
Puis ouvrir http://localhost:8765.

## Ajouter un projet
Dupliquer un bloc `<a class="card">` dans `index.html`, changer `href`, textes, icône et les couleurs `--accent` / `--accent-2` (format `R G B`). Mettre à jour le compteur `.count`.

## Déploiement GitHub Pages
1. Créer un repo GitHub et pousser ce dossier sur `main`.
2. Settings → Pages → Source : *Deploy from a branch*, `main` / `(root)`.
3. Le fichier `CNAME` contient déjà `zephyr1.fr`.
4. DNS chez le registrar de zephyr1.fr :
   - `A` @ → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `AAAA` @ (optionnel) → 2606:50c0:8000::153, 2606:50c0:8001::153, 2606:50c0:8002::153, 2606:50c0:8003::153
   - `CNAME` www → `<utilisateur>.github.io`
5. Une fois le DNS propagé, cocher « Enforce HTTPS ».
