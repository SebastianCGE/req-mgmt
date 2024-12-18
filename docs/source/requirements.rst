
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


Imported the following UML model from https://plantuml.com/sequence-diagram.

.. uml::
  Bob ->x Alice
  Bob -> Alice
  Bob ->> Alice
  Bob -\ Alice
  Bob \\- Alice
  Bob //-- Alice

  Bob ->o Alice
  Bob o\\-- Alice

  Bob <-> Alice
  Bob <->o Alice

Another UML model:

.. uml::
  package "Some Group" {
    HTTP - [First Component]
    [Another Component]
  }

  node "Other Groups" {
    FTP - [Second Component]
    [First Component] --> FTP
  }

  cloud {
    [Example 1]
  }


  database "MySql" {
    folder "This is my folder" {
      [Folder 3]
    }
    frame "Foo" {
      [Frame 4]
    }
  }


  [Another Component] --> [Example 1]
  [Example 1] --> [Folder 3]
  [Folder 3] --> [Frame 4]

Yet another UML Model, same as the first one....:

.. uml::

      User --> (Use)
      "Main Admin" as Admin
      "Compute BMI" as (Use)
      Admin --> (Install the application)

