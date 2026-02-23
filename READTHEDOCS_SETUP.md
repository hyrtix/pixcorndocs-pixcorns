# 📚 Configuration Read the Docs - pixcorns.com

## Étapes pour publier la documentation

### 1. Créer un compte Read the Docs

1. Allez sur https://readthedocs.org/
2. Cliquez sur "Sign Up"
3. Connectez-vous avec votre compte GitHub

### 2. Importer le projet

1. Une fois connecté, cliquez sur "Import a Project"
2. Sélectionnez le repo **pixcorndocs-pixcorns** dans la liste
3. Cliquez sur le bouton "+" à côté du repo

### 3. Configuration du projet

**Nom du projet**: `pixcorns-api-docs`

**Repository URL**: `https://github.com/VOTRE_USER/pixcorndocs-pixcorns`

**Default branch**: `main`

Cliquez sur "Next"

### 4. Configuration avancée (optionnel)

Dans les paramètres du projet (Admin → Advanced Settings):

- **Programming Language**: Python
- **Python Interpreter**: CPython 3.11
- **Requirements file**: `requirements.txt`
- **Documentation type**: Sphinx Html

### 5. Build automatique

Read the Docs va automatiquement:
- Détecter le fichier `.readthedocs.yaml`
- Installer les dépendances depuis `requirements.txt`
- Builder la documentation avec Sphinx
- Publier sur `https://pixcorns-api-docs.readthedocs.io/`

### 6. Domaine personnalisé (optionnel)

Pour utiliser `docs.pixcorns.com`:

1. Dans Read the Docs: Admin → Domains → Add Domain
2. Ajoutez `docs.pixcorns.com`
3. Configurez le DNS:
   ```
   CNAME docs.pixcorns.com → pixcorns-api-docs.readthedocs.io
   ```

### 7. Configuration DNS pixcorns.com

Pour le site principal, configurez ces enregistrements A :

| Type | Nom | Valeur |
|------|-----|--------|
| A | @ | 92.222.229.242 |
| A | www | 92.222.229.242 |
| A | api | 92.222.229.242 |
| A | checkout | 92.222.229.242 |

Voir `DNS_SETUP.md` pour les instructions détaillées.

## 🔄 Mises à jour automatiques

Chaque push sur `main` déclenchera automatiquement un rebuild de la documentation sur Read the Docs!

## 🌐 URLs

- **Documentation** : https://pixcorns-api-docs.readthedocs.io/
- **Site** : https://pixcorns.com
- **API** : https://api.pixcorns.com
- **Checkout** : https://checkout.pixcorns.com

## 📝 Modifier la documentation

1. Modifiez les fichiers `.rst` dans le repo
2. Commit et push
3. Read the Docs rebuild automatiquement
4. La doc est mise à jour en ~2 minutes
