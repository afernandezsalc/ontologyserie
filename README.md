# ontologyserie
ontología de serie de television
<?xml version="1.0"?>
<rdf:RDF xmlns="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#"
     xml:base="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv"
     xmlns:owl="http://www.w3.org/2002/07/owl#"
     xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
     xmlns:xml="http://www.w3.org/XML/1998/namespace"
     xmlns:xsd="http://www.w3.org/2001/XMLSchema#"
     xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#"
     xmlns:swrl="http://www.w3.org/2003/11/swrl#"
     xmlns:swrla="http://swrl.stanford.edu/ontologies/3.3/swrla.owl#"
     xmlns:swrlb="http://www.w3.org/2003/11/swrlb#"
     xmlns:terms="http://purl.org/dc/terms/"
     xmlns:serietv="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#">
    <owl:Ontology rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv">
        <terms:license rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Creative Commons Attribution 3.0 (CC BY 3.0)</terms:license>
        <rdfs:comment xml:lang="es">Television Series OWL Ontology  &quot;La que se Avecina&quot;

  Author: Antonio Fernández Salcedo</rdfs:comment>
        <rdfs:label xml:lang="en">Television_series</rdfs:label>
        <owl:versionInfo xml:lang="es">Version 1.0</owl:versionInfo>
    </owl:Ontology>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Annotation properties
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://purl.org/dc/terms/license -->

    <owl:AnnotationProperty rdf:about="http://purl.org/dc/terms/license"/>
    


    <!-- http://swrl.stanford.edu/ontologies/3.3/swrla.owl#isRuleEnabled -->

    <owl:AnnotationProperty rdf:about="http://swrl.stanford.edu/ontologies/3.3/swrla.owl#isRuleEnabled"/>
    


    <!-- http://www.w3.org/2000/01/rdf-schema#sameAs -->

    <owl:AnnotationProperty rdf:about="http://www.w3.org/2000/01/rdf-schema#sameAs">
        <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2000/01/rdf-schema#label"/>
    </owl:AnnotationProperty>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Object Properties
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasInterpretated -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasInterpretated">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AsymmetricProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:range rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Characters"/>
        <rdfs:comment xml:lang="es">La propiedad Interpretacción indica  el personaje que interpreta una persona de la Clase Person</rdfs:comment>
        <rdfs:label xml:lang="en">hasInterpretated</rdfs:label>
    </owl:ObjectProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasNameEpisodes -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasNameEpisodes">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SymmetricProperty"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#TransitiveProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdfs:range rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdfs:comment xml:lang="es">La propiedad Nombre de capitulo indica la nombre del capitulo</rdfs:comment>
        <rdfs:label xml:lang="en">hasNameEpisodes</rdfs:label>
    </owl:ObjectProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasPersonaje -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasPersonaje">
        <rdfs:subPropertyOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasInterpretated"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AsymmetricProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors"/>
        <rdfs:range rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Characters"/>
        <rdfs:comment xml:lang="es">La propiedad interpretacion de Personaje indica el Personje que interpreta  el actor de la clase Actors.</rdfs:comment>
        <rdfs:label xml:lang="en">hasPersonaje</rdfs:label>
    </owl:ObjectProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasYearSeasons -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasYearSeasons">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AsymmetricProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Year"/>
        <rdfs:range rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">La propiedad Años de las Temporadas indica el  año de cada Temporada (Seasons)</rdfs:comment>
        <rdfs:label xml:lang="en">hasYearSeasons</rdfs:label>
    </owl:ObjectProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hastitleEpisodes -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hastitleEpisodes">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AsymmetricProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        <rdfs:range rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdfs:comment xml:lang="es">La propiedad titulo de episodio indica el titulo de cada capitulo</rdfs:comment>
        <rdfs:label xml:lang="en">hasTitleEpisodes</rdfs:label>
    </owl:ObjectProperty>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Data properties
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitle -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitle">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
        <rdfs:comment xml:lang="es">La propiedad indica el nombre de un titulo</rdfs:comment>
        <rdfs:label xml:lang="en">nameTitle</rdfs:label>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitleEpisodes -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitleEpisodes">
        <rdfs:subPropertyOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitle"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
        <rdfs:comment xml:lang="es">La propiedad indica el nombre del titulo del episodio</rdfs:comment>
        <rdfs:label xml:lang="en">nameTitleEpisodes</rdfs:label>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitleSerie -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitleSerie">
        <rdfs:subPropertyOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#nameTitle"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
        <rdfs:comment xml:lang="es">La propiedad indica el nombre del titulo de la serie</rdfs:comment>
        <rdfs:label xml:lang="en">nameTitleSerie</rdfs:label>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberQuota -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberQuota">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
        <rdfs:comment xml:lang="es">La propiedad Numero de Cuota indica el porcentaje de la Audiencia</rdfs:comment>
        <rdfs:label xml:lang="en">numberQuota</rdfs:label>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberSpecteators -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberSpecteators">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
        <rdfs:comment xml:lang="es">La propiedad Numero de Espectadores indica el número de espectadores que tiene la audiencia.</rdfs:comment>
        <rdfs:label xml:lang="en">numberSpecteators</rdfs:label>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberseasons -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberseasons">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
        <rdfs:comment xml:lang="es">La propiedad Numero de Temporada indica el número de Temporada de la serie</rdfs:comment>
        <rdfs:label xml:lang="en">numberSeasons</rdfs:label>
    </owl:DatatypeProperty>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Classes
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Actores que puede tener instancias como el nombre de los actores</rdfs:comment>
        <rdfs:label xml:lang="en">Actors</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Audience -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Audience">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase de Tipo de Audiencia puede tener instancias como acumulada, bruta, duplicada</rdfs:comment>
        <rdfs:label xml:lang="en">Audience</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Premios, que puede tener instancias como mejor serie, mejor guion, mejor actor, mejor actriz, mejor serie de comedia, premio Sangay, premio Zapping, premio Pasión de Críticos</rdfs:comment>
        <rdfs:label xml:lang="en">Awards</rdfs:label>
        <rdfs:sameAs rdf:resource="https://dbpedia.org/page/Category:Television_series"/>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Medios de difusion que puede tener instancias como Telecinco, Amazon Prime Video, Disney +, Netflix, Atresplayer, YouTube</rdfs:comment>
        <rdfs:label xml:lang="en">BroadcastMedium</rdfs:label>
        <rdfs:sameAs rdf:resource="https://dbpedia.org/page/Category:Series"/>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Characters -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Characters">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Personajes puede tener instancia del personaje que se relaciona con el actor</rdfs:comment>
        <rdfs:label xml:lang="en">Characters</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <owl:disjointWith rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor"/>
        <rdfs:comment xml:lang="es">Clase Comedia que puede tener instancias como comedia de situación</rdfs:comment>
        <rdfs:label xml:lang="en">Comedy</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Pais de origen que puede tener instacia como Spain</rdfs:comment>
        <rdfs:label xml:lang="en">CountryOrigin</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Creadores que puede tener instancias con el nombre de los creadores</rdfs:comment>
        <rdfs:label xml:lang="en">Creators</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Directors -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Directors">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Directores que puede tener instancias con el nombre de los directores</rdfs:comment>
        <rdfs:label xml:lang="en">Directors</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Episodios puede tener instancias como número de episodio 11</rdfs:comment>
        <rdfs:label xml:lang="en">Episodes</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Final, que identifica la fecha de final de emision de la Temporada, puede tener una instancia como 22 de julio de 2007</rdfs:comment>
        <rdfs:label xml:lang="en">Final</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Generos que puede tener instancias genericas de los diferentes generos y mas ordenadamente tiene las subclases de Comedy y Humor</rdfs:comment>
        <rdfs:label xml:lang="en">Genders</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <rdfs:comment xml:lang="es">Clase Humor que puede tener instacias como humor negro</rdfs:comment>
        <rdfs:label xml:lang="en">Humor</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Lenguaje original que tiene instancia como Spanish</rdfs:comment>
        <rdfs:label xml:lang="en">OriginalLanguage</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Person que tiene subclases (Actores, Creadores, Directores, Productores, Guionista)</rdfs:comment>
        <rdfs:label xml:lang="en">Person</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Estreno que puede tener una instancia con la fecha de estreno de la temporada como 22 de abril de 2007</rdfs:comment>
        <rdfs:label xml:lang="en">Premier</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Productores que puede tener instancias con el nombre de los productores</rdfs:comment>
        <rdfs:label xml:lang="en">Producers</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Couta puede tener instancia como 23.3 %</rdfs:comment>
        <rdfs:label xml:lang="en">Quota</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Screenwriters -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Screenwriters">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Guionistas que pueden tener instancias con el nombre de los guionistas</rdfs:comment>
        <rdfs:label xml:lang="en">Screenwriters</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Temporadas, puede tener instancias como Temporada 4 (2009-2010), Temporada 12(2020-2022)</rdfs:comment>
        <rdfs:label xml:lang="en">Seasons</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Espectadores puede tener una instacia como 3.185.000</rdfs:comment>
        <rdfs:label xml:lang="en">Spectators</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Titulo que puede tener instancia como La que se Avecina que es el titulo de la serie, o el titulo de un Capitulo</rdfs:comment>
        <rdfs:label xml:lang="en">Title</rdfs:label>
        <rdfs:sameAs rdf:resource="https://dbpedia.org/page/Television_show"/>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Year -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Year">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Año que puede incluir un instancia con un año</rdfs:comment>
        <rdfs:label xml:lang="en">Year</rdfs:label>
    </owl:Class>
    


    <!-- http://www.w3.org/2002/07/owl#SerieTV -->

    <owl:Class rdf:about="http://www.w3.org/2002/07/owl#SerieTV">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
        <rdfs:comment xml:lang="es">Clase Serie de Television</rdfs:comment>
        <rdfs:label xml:lang="en">SerieTV</rdfs:label>
    </owl:Class>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Individuals
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Alberto_Caballero -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Alberto_Caballero">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Screenwriters"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Amazon_Prime_Video -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Amazon_Prime_Video">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Atresplayer -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Atresplayer">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedia_de_situacion -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedia_de_situacion">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor_negro -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor_negro">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Jordi_Sánchez -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Jordi_Sánchez">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#La_que_se_Avecina -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#La_que_se_Avecina">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Laura_Caballero -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Laura_Caballero">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Directors"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Netflix -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Netflix">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spain -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spain">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spanish -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spanish">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Telecinco -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Telecinco">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#11-07-15 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#11-07-15">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#12-09-16 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#12-09-16">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2.019 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2.019">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Year"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2014.Premio_MiM_Series.Mejor_serie_de_comedia -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2014.Premio_MiM_Series.Mejor_serie_de_comedia">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_guion. -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_guion.">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_serie -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_serie">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#23.2 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#23.2">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3.000.000 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3.000.000">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Disney_+ -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Disney_+">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
    </owl:NamedIndividual>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // General axioms
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    <rdf:Description>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AllDisjointClasses"/>
        <owl:members rdf:parseType="Collection">
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Audience"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators"/>
        </owl:members>
    </rdf:Description>
    <rdf:Description>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AllDisjointClasses"/>
        <owl:members rdf:parseType="Collection">
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        </owl:members>
    </rdf:Description>
    <rdf:Description>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AllDisjointClasses"/>
        <owl:members rdf:parseType="Collection">
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        </owl:members>
    </rdf:Description>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Rules
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p">
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Variable"/>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S1</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S3</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                        <rdf:first>
                            <rdf:Description>
                                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                                <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor"/>
                                <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                            </rdf:Description>
                        </rdf:first>
                        <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
                    </rdf:Description>
                </rdf:rest>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S2</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S4</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Description>
</rdf:RDF>



<!-- Generated by the OWL API (version 4.5.9.2019-02-01T07:24:44Z) https://github.com/owlcs/owlapi -->

