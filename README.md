## If you are interested in access to our data, note that links are only downloadable by registered users.
## To obtain an access, please contact us at data.orphanet@inserm.fr.


# RDCO-Triplestores.
Here are the links in order to download archives files of the two RDCO ontologies (e.g RDCO_PHENO and RDCO_ORDO) in OWL format:

     - http://www.orphadata.org/data/SOLVE-RD/Triplestore/RDCO_ORDO_Oct2019.zip
     - http://www.orphadata.org/data/SOLVE-RD/Triplestore/RDCO_PHENO_Oct2019.zip
     
 # RDCO-Sparql-Endpoints.
 Here the links in order to download archives files of Sparql Enpoints available and/or needed to querying RDCO ontologies:
 
     - http://www.orphadata.org/data/SOLVE-RD/SparqlEndpoints/JenaRDCO_ORDO_8010_Oct2019.zip
     - http://www.orphadata.org/data/SOLVE-RD/SparqlEndpoints/JenaRDCO_PHENO_8020_Oct2019.zip
     - http://www.orphadata.org/data/SOLVE-RD/SparqlEndpoints/OrdoBlazeGraph.zip
     - http://www.orphadata.org/data/SOLVE-RD/SparqlEndpoints/HOOMBlazeGraph.zip
     

     
 ## How to run and query Sparql-Endpoints.
 1. Unzip the archives files.
 2. Two differents technologies were employed, **Jena TBD Fuseki** server for **RDCO** and **Blazegraph** for **ORDO** and **HOOM**.
     - For Jena, in the dedicated folder (JenaRDCO_ORDO_8010_collection or JenaRDCO_PHENO_8020_collection), one can find a startFuseki.bat file containing the command line capable to launch the server on a Windows OS.
     Otherwise, you can run in a terminal the command line :  
            
            java -jar fuseki-server.jar --port=8010 --update --loc=data /ds
     Note: if you want to run federated queries, beware to use differents ports for differents sparql endpoints (8010 for RDCO-ORDO and 8020 for RDCO-PHENO).                    
    
    - For Blazegraph, in the dedicated folder (OrdoBlazeGraph or HOOMBlazeGraph), one can find a startBlazeGraph.bat file containing the command line capable to launch the server on a Windows OS.
     Otherwise, you can run in a terminal the command line :   
            
            java -server -Xmx4g -Djetty.port=9990 -jar blazegraph.jar  
            
3. To query the sparql endpoints, in a browser open: 
     
     **for JenaRDCO_ORDO_8010_collection**
            
            http://localhost:8010/   
            
      **for JenaRDCO_PHENO_8020_collection**
      
            http://localhost:8020/
      
      **for OrdoBlazeGraph**       
      
            http://192.168.0.108:9999/blazegraph/#splash
          
      **for HOOMBlazeGraph**       
      
            http://192.168.0.108:9990/blazegraph/#splash
            
            
            
       
