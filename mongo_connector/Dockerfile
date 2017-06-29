FROM python:3-slim

RUN pip install neo4j-doc-manager

ENV MONGO_HOST=localhost MONGO_PORT=27017 NEO4J_HOST=localhost NEO4J_PORT=7474

CMD mongo-connector -m $MONGO_HOST:$MONGO_PORT -t http://$NEO4J_HOST:$NEO4J_PORT/db/data -d neo4j_doc_manager
