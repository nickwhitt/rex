# REX

A graph database for European monarchies and ancestors.

## Import

    docker-compose exec neo4j bin/neo4j-admin import \
        --database=monarchy \
        --nodes=Person=import/people.csv \
        --nodes=Dynasty=import/dynasties.csv \
        --nodes=Kingdom=import/kingdoms.csv \
        --relationships=import/houses.csv \
        --relationships=import/ancestors.csv \
        --relationships=import/monarchies.csv \
        --relationships=import/successions.csv
