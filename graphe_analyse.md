# Box plot

Un box plot, également connu sous le nom de boîte à moustaches, est un graphique statistique utilisé pour représenter la distribution des données numériques. Il fournit un aperçu de plusieurs caractéristiques clés de la distribution, notamment la médiane, les quartiles, les valeurs aberrantes potentielles et la plage interquartile. Voici comment un box plot fonctionne et comment l'interpréter :

**Composants d'un Box Plot :**

1. **Boîte (Box) :** La boîte représente le deuxième et troisième quartiles de la distribution, c'est-à-dire la médiane (Q2) et la plage interquartile (IQR, Q3 - Q1). La longueur de la boîte indique la variabilité des données au sein de cette plage.

2. **Médiane (Median) :** La ligne à l'intérieur de la boîte représente la médiane, qui est la valeur qui divise la distribution en deux parties égales.

3. **Moustaches (Whiskers) :** Les moustaches s'étendent à partir de la boîte et vont jusqu'aux valeurs extrêmes, mais elles ne dépassent généralement pas un certain multiple de l'IQR. Les valeurs situées au-delà des moustaches sont considérées comme des valeurs aberrantes potentielles.

4. **Valeurs Aberrantes (Outliers) :** Les points situés en dehors des moustaches sont souvent marqués comme des valeurs aberrantes potentielles. Cela signifie qu'ils se trouvent à une distance anormalement grande de la médiane.

**Interprétation d'un Box Plot :**

1. **Position de la Médiane :** La position de la médiane dans la boîte indique la tendance centrale de la distribution. Si la médiane est près du centre de la boîte, la distribution est symétrique. Si elle est plus proche d'une extrémité, la distribution est biaisée.

2. **Variabilité :** La longueur de la boîte (hauteur de la boîte) indique la variabilité des données. Une boîte plus longue suggère une variabilité plus importante.

3. **Étendue :** Les moustaches indiquent la plage des valeurs non aberrantes. Si les moustaches sont longues, la plage des données est large.

4. **Valeurs Aberrantes :** Les valeurs situées au-delà des moustaches sont marquées comme des valeurs aberrantes potentielles. Ces valeurs peuvent être importantes, car elles se trouvent à une distance significative de la médiane.

5. **Comparaison :** Les box plots sont particulièrement utiles pour comparer les distributions de plusieurs groupes ou catégories. Vous pouvez facilement visualiser les différences dans la tendance centrale, la variabilité et la présence de valeurs aberrantes entre les groupes.

## Dessin

Pour dessiner un box plot en utilisant Python, vous pouvez utiliser la bibliothèque Matplotlib ou Seaborn. Voici comment créer un box plot à l'aide de Matplotlib :

```python
import matplotlib.pyplot as plt

# Données à représenter (par exemple, une liste de valeurs numériques)
data = [15, 20, 30, 35, 40, 45, 50, 55, 60, 70]

# Création du box plot
plt.boxplot(data)

# Ajout de titres et d'étiquettes
plt.title("Box Plot")
plt.xlabel("Données")
plt.ylabel("Valeurs")

# Affichage du graphique
plt.show()
```

Ce code crée un box plot basique en utilisant Matplotlib pour les données fournies. Vous pouvez personnaliser davantage le graphique en ajoutant des titres, des étiquettes d'axe, des couleurs, etc.

Si vous préférez utiliser Seaborn, voici comment créer un box plot avec cette bibliothèque :

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Données à représenter (par exemple, une liste de valeurs numériques)
data = [15, 20, 30, 35, 40, 45, 50, 55, 60, 70]

# Création du box plot avec Seaborn
sns.boxplot(data)

# Ajout de titres et d'étiquettes
plt.title("Box Plot")
plt.xlabel("Données")
plt.ylabel("Valeurs")

# Affichage du graphique
plt.show()
```

Utiliser Seaborn peut rendre la création de box plots plus simple et permet de personnaliser le style du graphique plus facilement.

Assurez-vous d'adapter le code aux données que vous souhaitez représenter. Vous pouvez fournir une liste de valeurs numériques ou un jeu de données à la place de "data" dans les exemples ci-dessus.