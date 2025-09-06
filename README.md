# Flor-Trial
Trials for exam
# Sala Rossa

## SPARQL ASK Query
```sparql
PREFIX arco-core: <https://w3id.org/arco/ontology/core/>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

ASK { 
  { <https://w3id.org/arco/resource/ArchitecturalOrLandscapeHeritage/SalaRossa_PalazzoAccursio> 
      arco-core:isPartOf <https://w3id.org/arco/resource/ArchitecturalOrLandscapeHeritage/0800262039> ; 
      rdfs:label "Sala Rossa"@it . }
  UNION
  { <https://w3id.org/arco/resource/ArchitecturalOrLandscapeHeritage/0800262039> 
      arco-core:hasPart <https://w3id.org/arco/resource/ArchitecturalOrLandscapeHeritage/SalaRossa_PalazzoAccursio> . 
    <https://w3id.org/arco/resource/ArchitecturalOrLandscapeHeritage/SalaRossa_PalazzoAccursio> rdfs:label "Sala Rossa"@it . }
}
