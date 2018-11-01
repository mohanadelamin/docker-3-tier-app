This is a working example of a 3-tier flask application with Postgres as the database and the nginx reverse proxy as frontend.

## Setup 
The setup look like the following:
```bash
+-------------+                +-------------+               +-------------+
|             |    +------+    |             |    +-----+    |             |
|    Nginx    +----+web_nw+----+  Flask App  +----+db_nw+----+ Postgres DB |
|             |    +------+    |             |    +-----+    |             |
+-------------+                +-------------+               +-------------+
```

## Usage

1. Clone the repo using:
```bash
git clone https://github.com/mohanadelamin/docker-3-tier-app
```

2. Run the containers
```bash
$ docker-compose up --build -d
```

3. Browse to localhost:8080 to see the app in action.

To remove everything use the following command:
```bash
$ docker-compose down
```

## Example output

![Example output](https://raw.githubusercontent.com/mohanadelamin/docker-3-tier-app/master/exmple_output.png)
