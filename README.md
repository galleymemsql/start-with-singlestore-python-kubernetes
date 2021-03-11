Getting started with SingleStore and Python on Kubernetes
=========================================================


Whether you're using an ORM or straight SQL, you can get started with SingleStore (formerly MemSQL) fast. Here's an introductory sample of using SingleStore with Python. This sample includes all the CRUD methods: Create, Read by id, Read all, Update, and Delete.

Note that this is only for local development. If you're looking for a production Kubernetes installation, look to the SingleStore Kubernetes Operator.


Usage
-----

1. [Sign up](https://msql.co/2E8aBa2) for a free SingleStore license. This allows you to run up to 4 nodes up to 32 gigs each for free.

2. Spin up a developer SingleStore cluster.

   Grab your license key from [SingleStore portal](https://msql.co/3fZoxjO) and set it into `kubernetes.yaml`
   
   Run `kubectl apply -f kubernetes.yaml` to start the cluster.

3. Connect to SingleStore Studio and run `init.sql`:

   Open http://localhost:30080/, login with username `root` and the password you set in `kubernetes.yaml`.

   Switch to the SQL Editor tab.

   Copy the contents of `init.sql`, and run all the statements.

4. Adjust the connection details in `main.py`, `pip install -r requirements.txt`, and run `python main.py`.


License
-------

MIT
