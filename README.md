# Swagger merger

To merge a few swagger JSON files into one.

Install the command line tool first.

	go get github.com/murouse/go-swagger-merger

The command below will merge ``/data/swagger1.json`` ``/data/swagger2.json`` and save result file in the ``/data/swagger.json``. The library supports more than two files to merge. You can add more paths to the list ``/data/swagger3.json``, ``/data/swaggerN.json``.

	go-swagger-merger -o /data/swagger.json -t your_title -v your_version /data/swagger1.json /data/swagger2.json

Attention. The order of the files is essential, and the following file overwrites the same fields from the previous file.
