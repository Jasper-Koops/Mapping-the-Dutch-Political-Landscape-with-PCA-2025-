<style>
figure {
  page-break-inside: avoid;
  text-align: center;
  margin: 2em auto;
}
figure figcaption {
  font-weight: bold;
  font-size: 1.3em;
  margin-bottom: 0.4em;
}
img {
  max-width: 80%;
  height: auto;
  display: block;
  margin: 0 auto;
}
</style>

# 1. Hoofdcomponentenanalyse

Hoofdcomponentenanalyse (PCA) is een statistische techniek die wordt gebruikt voor dimensionale reductie. Dit is een methode  waarmee de dimensies of variabelen van een dataset worden verminderd, terwijl zo veel mogelijk relevante informatie behouden blijft. Het doel is om de complexiteit van gegevens te verminderen door de dataset om te zetten in een lagere-dimensionale ruimte, terwijl belangrijke patronen en relaties in de gegevens behouden blijven.

De overgebleven dimensies, de 'hoofdcomponenten' zijn combinaties van de oorspronkelijke variabelen en kunnen worden gebruikt om de belangrijkste patronen in de data te identificeren. Hierdoor wordt het mogelijk om de data te visualiseren in een grafiek met minder dimensies. Niet elk component verklaart evenveel van de variantie in de data. De eerste component verklaart de meeste variantie, de tweede component verklaart de meeste variantie van de overgebleven variantie, enzovoort. De toegevoegde waarde van een component neemt hierdoor af naarmate er meer componenten worden toegevoegd, omdat elk nieuw component een kleiner deel van de totale variantie verklaart.


# 2. Analyse stemhulpen

Dit is een analyse van hoe de verschillende partijen zich tot elkaar verhouden op basis van de stellingen uit de stemhulpen. Het doel is om hierdoor een beter beeld te kunnen geven van het antwoord op vragen als: "Waar bevindt de NSC zich op het politieke spectrum?", "Hoeveel overlap is er tussen de partijen?".

Elke vraag in een stemhulp vertegenwoordigt een dimensie, dit betekent dat een stemhulp met dertig vragen een dertigdimensionale dataset oplevert. Om deze data alsnog te kunnen visualiseren is er een hoofdcomponentenanalyse toegepast op de gegevens van alle stemhulpen om het aantal dimensies terug te brengen tot één, twee of drie dimensies. Hierdoor is het mogelijk de posities van de partijen in een grafiek weer te geven. Partijen die zich dicht bij elkaar bevinden zijn het met elkaar eens, partijen die ver van elkaar afstaan, verschillen sterker van mening. Het is belangrijk te beseffen dat niet elke as (of 'component') evenveel van de variantie verklaart. In de grafieken staat per as aangegeven welk deel van de variantie wordt verklaard en dus ook hoe 'belangrijk' deze as is.

Per component is er een analyse gemaakt van de stellingen die de grootste invloed hebben op de positie van de partijen. Hierdoor wordt inzichtelijk gemaakt wat een as in de grafiek representeert. De antwoorden van de partijen op de stellingen zijn gecodeerd als getallen. Hoe hoger het getal, hoe meer de partij het eens is met de stelling, negatieve waarden betekenen dat de partij het oneens is met de stelling. Deze antwoorden worden vermenigvuldigd met de waarden ('loadings') die de stellingen hebben voor het betreffende component. De som van deze vermenigvuldigingen bepaalt de positie van de partij op dat component.

Tot slot heb ik de correlatie tussen de antwoorden van de partijen berekend. Hoe hoger de correlatie, hoe groter de mate waarin de partijen het met elkaar eens zijn.

# Kieskompas en Stemwijzer gecombineerd

<figure>
  <img src="images/combined/scree.png"
       alt="Scree plot gecombineerde data">
  <figcaption>Scree plot — verklaarde variantie per component.</figcaption>
</figure>

<figure>
  <img src="images/combined/pca-scatter-1d.png"
       alt="PCA 1D - gecombineerde data">
  <figcaption>PCA 1D - gecombineerde data</figcaption>
</figure>

<figure>
    <img src="images/combined/pca-scatter-2d.png"
         alt="PCA 2D - gecombineerde data">
    <figcaption>PCA 2D - gecombineerde data</figcaption>
</figure>

<figure>
    <img src="images/combined/pca-scatter-3d.png"
         alt="PCA 3D - gecombineerde data">
    <figcaption>PCA 3D - gecombineerde data</figcaption>
</figure>

<figure>
    <img src="images/combined/loadings-graph-pca1.png"
         alt="Loadings component 1 - gecombineerde data">
    <figcaption>Loadings component 1 - gecombineerde data</figcaption>
</figure>

<figure>
    <img src="images/combined/loadings-graph-pca2.png"
         alt="Loadings component 2 - gecombineerde data">
    <figcaption>Loadings component 2 - gecombineerde data</figcaption>
</figure>

<figure>
    <img src="images/combined/corr-graph.png"
         alt="Correlatie tabel - gecombineerde data">
    <figcaption>Correlatie tabel - gecombineerde data</figcaption>
</figure>

# Kieskompas

<figure>
  <img src="images/kieskompas/scree.png"
       alt="Scree plot kieskompas">
  <figcaption>Scree plot — verklaarde variantie per component.</figcaption>
</figure>

<figure>
  <img src="images/kieskompas/pca-scatter-1d.png"
       alt="PCA 1D - kieskompas">
  <figcaption>PCA 1D - kieskompas</figcaption>
</figure>

<figure>
    <img src="images/kieskompas/pca-scatter-2d.png"
         alt="PCA 2D - kieskompas">
    <figcaption>PCA 2D - kieskompas</figcaption>
</figure>

<figure>
    <img src="images/kieskompas/pca-scatter-3d.png"
         alt="PCA 3D - kieskompas">
    <figcaption>PCA 3D - kieskompas</figcaption>
</figure>

<figure>
    <img src="images/kieskompas/loadings-graph-pca1.png"
         alt="Loadings component 1 - kieskompas">
    <figcaption>Loadings component 1 - kieskompas</figcaption>
</figure>

<figure>
    <img src="images/kieskompas/loadings-graph-pca2.png"
         alt="Loadings component 2 - kieskompas">
    <figcaption>Loadings component 2 - kieskompas</figcaption>
</figure>

<figure>
    <img src="images/kieskompas/corr-graph.png"
         alt="Correlatie tabel - kieskompas">
    <figcaption>Correlatie tabel - kieskompas</figcaption>
</figure>

# Stemwijzer

<figure>
  <img src="images/stemwijzer/scree.png"
       alt="Scree plot stemwijzer">
  <figcaption>Scree plot — verklaarde variantie per component.</figcaption>
</figure>

<figure>
  <img src="images/stemwijzer/pca-scatter-1d.png"
       alt="PCA 1D - stemwijzer">
  <figcaption>PCA 1D - stemwijzer</figcaption>
</figure>

<figure>
    <img src="images/stemwijzer/pca-scatter-2d.png"
         alt="PCA 2D - stemwijzer">
    <figcaption>PCA 2D - stemwijzer</figcaption>
</figure>

<figure>
    <img src="images/stemwijzer/pca-scatter-3d.png"
         alt="PCA 3D - stemwijzer">
    <figcaption>PCA 3D - stemwijzer</figcaption>
</figure>

<figure>
    <img src="images/stemwijzer/loadings-graph-pca1.png"
         alt="Loadings component 1 - stemwijzer">
    <figcaption>Loadings component 1 - stemwijzer</figcaption>
</figure>

<figure>
    <img src="images/stemwijzer/loadings-graph-pca2.png"
         alt="Loadings component 2 - stemwijzer">
    <figcaption>Loadings component 2 - stemwijzer</figcaption>
</figure>

<figure>
    <img src="images/stemwijzer/corr-graph.png"
         alt="Correlatie tabel - stemwijzer">
    <figcaption>Correlatie tabel - stemwijzer</figcaption>
</figure>
