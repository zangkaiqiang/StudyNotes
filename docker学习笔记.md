## docker run 
docker run -it --rm images bash

## docker commit
docker commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]
OPTIONS:
--author , -a		Author (e.g., “John Hannibal Smith hannibal@a-team.com”)
--change , -c		Apply Dockerfile instruction to the created image
--message , -m		Commit message
--pause , -p	true	Pause container during commit
EXAMPLE:
docker commit -m "update" container_id zangkaiqiang/commit_test:v2
