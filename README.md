<img width="923" height="520" alt="Screenshot 2026-04-05 at 7 23 51 PM" src="https://github.com/user-attachments/assets/5a455e79-6c16-41da-a3f8-30581ebf3225" />
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


        
