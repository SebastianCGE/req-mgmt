
Requirements 
============

  .. todo:: The requirements list does not yet pretend to be complete and will be extended over time.

  Overview Requirements
  ----------------------
    
  .. needtable::
    :types: req
    :columns: id;title;incoming
    :style: datatable
    
  Detailed Requirements
  -----------------------

  .. req:: The product shall compute the BMI
    :id: R_compute_bmi

    The product shall be capable of computing the BMI of a person

    .. uml::

      User --> (Use)
      "Main Admin" as Admin
      "Compute BMI" as (Use)
      Admin --> (Install the application)

  .. req:: The product shall be version controlled
    :id: R_version_controlled

    The product shall be version controlled using a distributed version control system 

  .. req:: The product shall be user friendly
    :id: R_user_friendly
    :links: R_version_controlled, R_cheap, R_compute_bmi

    The product shall be user friendly for adults

  .. needimport:: cheap.json


Imported the following model from https://plantuml.com/sequence-diagram.

.. uml::
  autonumber
  Bob -> Alice : Authentication Request
  Bob <- Alice : Authentication Response

  autonumber 15
  Bob -> Alice : Another authentication Request
  Bob <- Alice : Another authentication Response

  autonumber 40 10
  Bob -> Alice : Yet another authentication Request
  Bob <- Alice : Yet another authentication Response




