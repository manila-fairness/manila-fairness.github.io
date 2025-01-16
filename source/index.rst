.. MANILA documentation master file, created by
   sphinx-quickstart on Wed Nov 15 15:00:43 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to MANILA's documentation!
==================================

**MANILA** is a low-code web-application to benchmark the *fairness* and *effectiveness* of machine learning models and fairness enhancing methods.

Installation
------------

To install MANILA, you can use the following command:

**Using Docker**

To run the application using Docker, execute the following command:

.. code-block:: bash

    docker-compose up

The application will be available at `http://localhost:3000`.

**Manually**

To run the application manually, follow the steps below:

1. Install the dependencies of the backend:

.. code-block:: bash
   
   cd app
   pip install -r requirements.txt


2. Install and launch the Redis database (refer to the official documentation (https://redis.io/download) for more information).

3. Launch the backend:

.. code-block:: bash

   cd app
   python manila/app.py


4. Launch the Celery worker:

.. code-block:: bash
   
   cd app/manila
   celery -A run_celery.celery worker --loglevel=info


5. Install the dependencies of the frontend:

.. code-block:: bash
   
   cd frontend
   npm install


6. Launch the frontend:

.. code-block:: bash
   
   cd frontend
   npm start


The application will be available at `http://localhost:3000`.



.. It is freely available as a web-application in the `SoBigData Research Infrastructure <https://sobigdata.d4science.org/group/sobigdata.it/manila-univaq>`_.

Citation Request
----------------

Please cite our work if you use MANILA in your research:

*d’Aloisio, G., Di Marco, A., Stilo, G. (2023). Democratizing Quality-Based Machine Learning Development through Extended Feature Models. In: Lambers, L., Uchitel, S. (eds) Fundamental Approaches to Software Engineering. FASE 2023. Lecture Notes in Computer Science, vol 13991. Springer, Cham.* `<https://doi.org/10.1007/978-3-031-30826-0_5>`_

.. code-block:: bibtex

   @inproceedings{d2023democratizing,
      title={Democratizing Quality-Based Machine Learning Development through Extended Feature Models},
      author={d’Aloisio, Giordano and Di Marco, Antinisca and Stilo, Giovanni},
      booktitle={International Conference on Fundamental Approaches to Software Engineering},
      pages={88--110},
      year={2023},
      doi={10.1007/978-3-031-30826-0_5},
      organization={Springer Nature Switzerland Cham}
   }


Contents
--------
.. toctree::
   tutorial/index
   :maxdepth: 2
..   usage



.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`search`
