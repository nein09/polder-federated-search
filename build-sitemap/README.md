This folder contains the necessary Dockerfile and script needed to query DataCite for DOIs associated with an organization, generate a sitemap from it, and place that sitemap in Minio, where Gleaner can then use it to crawl those DOIs, as if they were all on one website.

The docker image is currently published on Docker Hub as nein09/build-bas-sitemap. It could be used to build other sitemaps as well. It contains an instance of Minio Client, curl, jq, and bash.

Build the image by doing `docker build  --tag nein09/build-bas-sitemap .`
