# Big-Data-Modelling-and-Management

C:\Users\catar>docker stop Neo4JHW2025
Neo4JHW2025

C:\Users\catar>docker rm Neo4JHW2025
Neo4JHW2025

C:\Users\catar>docker run --name Neo4JHW2025 -p 7474:7474 -p 7687:7687 -d -v "C:\Users\catar\Desktop\big-data-modeling\Neo4JPlugins":/plugins -v "C:\Users\catar\Desktop\big-data-modeling\Neo4JHWData\NEW_VERSION\data":/data --env NEO4J_AUTH=neo4j/test --env NEO4J_dbms_connector_https_advertised__address="localhost:7473" --env NEO4J_dbms_connector_http_advertised__address="localhost:7474" --env NEO4J_dbms_connector_bolt_advertised__address="localhost:7687" --env NEO4J_dbms_security_procedures_unrestricted=gds.* --env NEO4J_dbms_security_procedures_allowlist="gds.*" neo4j:4.4.5
9ad48e239b0973b87d980186001321e69c23ad9f00b9a4ed78b21d6b7d7c97bf

C:\Users\catar>docker ps
CONTAINER ID   IMAGE         COMMAND                  CREATED          STATUS          PORTS                                                      NAMES
9ad48e239b09   neo4j:4.4.5   "tini -g -- /startup…"   35 seconds ago   Up 34 seconds   0.0.0.0:7474->7474/tcp, 7473/tcp, 0.0.0.0:7687->7687/tcp   Neo4JHW2025

http://localhost:7474/browser/http://localhost:7474/browser/
