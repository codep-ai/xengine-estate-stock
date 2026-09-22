# xengine-estate-stock

The shared contract between the team repos of the multi-project cross-engine demo: `estate.yml` lists the projects, the engine
that builds each, the catalog sync the producer needs, and the pipeline id under which the stitched lineage is stored.

    X=/home/ec2-user/git/datapai-platform-be
    python $X/scripts/xengine.py snowflake-sync --estate estate.yml
    python $X/scripts/xengine.py lineage        --estate estate.yml --to-db
