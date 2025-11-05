# Tuto Blender – Séparer les parties du modèle (simple)

## 1. Exporter depuis Roblox

1. Dans **Roblox Studio → Explorer** : clic droit sur le modèle  
2. **Save/Export → Export Selection**  
3. Choisis un dossier (tu obtiens : `.obj`, `.mtl`, texture)

---

## 2. Importer dans Blender

1. Ouvre Blender → nouveau fichier **General**  
2. Dans la vue 3D :  
   - `A` → tout sélectionner  
   - `X` → **Delete**  
3. **File → Import → Wavefront (.obj)**  
   - Va dans le dossier exporté  
   - Sélectionne le `.obj` → **Import OBJ**

---

## 3. Passer en Edit Mode et préparer la sélection

1. Sélectionne ton objet (clic gauche)  
2. `Tab` → passe en **Edit Mode**  
3. En haut de la vue 3D, clique sur l’icône **Face Select** (le petit carré)  

### Activer/Désactiver X-Ray (sans Alt+Z)

- En haut à droite de la vue 3D : clique sur l’icône avec **deux carrés superposés** → **X-Ray** on/off  
- Ou `Z` → choisir **X-Ray** dans le menu en cercle

---

## 4. Séparer les parties (jambes, pieds, etc.)

1. En Edit Mode + Face Select :  
   - `C` → **Circle Select**  
2. Clique/peins sur les faces de la partie à isoler (jambe, pied, bras, etc.)  
3. Quand la sélection est prête :  
   - `P` → **Selection**  

:arrow_right: Ça crée un **nouvel objet** pour cette partie.

---

## 5. UV

1. `U` → **Smart UV Project**  
2. Valide

---

## 6. Plugin Vertex Color / Bake

1. Dans la vue 3D : `N` → ouvre le panneau à droite  
2. Va dans l’onglet du plugin (**Vertex Color** par exemple)  
3. Dans **Collection**, sélectionne ta collection  
4. Règle brightness, saturation, etc.  
5. Clique sur **Bake All**

---

## 7. Séparer par matériau (By Material)

1. Dans l’**Outliner** (liste des objets) : sélectionne tous les objets à traiter  
2. `Tab` → passe en **Edit Mode** (multi-objets)  
3. `A` → tout sélectionner  
4. `P` → **By Material**

Chaque matériau devient un objet séparé.

---

## 8. Export en FBX

1. `Tab` → reviens en **Object Mode**  
2. Sélectionne les objets à exporter  
3. **File → Export → FBX (.fbx)**  
4. Coche **Selected Objects**  
5. Choisis le dossier + nom → **Export FBX**

---

## Raccourcis utiles

- `Tab` : Object Mode ↔ Edit Mode  
- `A` : tout sélectionner  
- `C` : Circle Select  
- `P` : Separate (Selection / By Material)  
- `U` : menu UV → Smart UV Project  
- `Z` : menu d’affichage (dont X-Ray)
