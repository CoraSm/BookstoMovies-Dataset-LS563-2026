<img width="1520" height="842" alt="image" src="https://github.com/user-attachments/assets/c35b5b0c-98fc-4e26-8dc0-9de45a87cc62" />

<img width="1160" height="372" alt="Screenshot 2026-04-05 at 7 37 55 PM" src="https://github.com/user-attachments/assets/7e08f402-6672-4bd0-8e4f-e6b9b84a3cc0" />

**Dataset Description**
This dataset represents books that have been adapted into movies, with release dates included, as well as authors and directors.

**Ontologies and Vocabuliaries Used**
RDF Schema
Schema.org
XSD
VIAF
WikiData

**Linking Strategies**
WikiData and VIAF were used to link book titles, authors, movie titles, and directors to link to external authority datasets.

**Sample Triples**
@prefix : <http://localhost:3333/> .
@prefix schema: <http://schema.org/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
@prefix wd: <http://www.wikidata.org/entity/> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix viaf: <https://viaf.org/en/viaf/> .

:TheGiver  schema:isBasedOn   wd:Q258953 ;
        schema:datePublished  "2014"^^xsd:gYear ;
        schema:director       wd:Q543563 ;
        schema:name           "The Giver" ;
        rdf:type              schema:Movie .

:Matilda  schema:isBasedOn    wd:Q1426188 ;
        schema:datePublished  "1996"^^xsd:gYear ;
        schema:director       wd:Q26806 ;
        schema:name           wd:Q280400 ;
        rdf:type              schema:Movie .

:TheSecretLifeofBees  schema:isBasedOn  wd:Q3435184 ;
        schema:datePublished  "2008"^^xsd:gYear ;
        schema:director       wd:Q3106705 ;
        schema:name           wd:Q940387 ;
        rdf:type              schema:Movie .



