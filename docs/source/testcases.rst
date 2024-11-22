
Test Cases 
================

Overview Test Cases 
------------------------
   
.. needtable::
  :types: test, Test-Case
  :columns: id;title;result;incoming;outpoing
  :style: table
   
Detailed Test Cases 
-------------------------

.. test:: Test if version controlled
  :id: T_version_controlled
  :tags: system
  :status: open
  :links: I_version_controlled, R_version_controlled

.. test:: Test if user friendly
  :id: T_user_friendly
  :tags: system
  :status: open
  :links: I_user_friendly, R_user_friendly

Test Cases with link to automated tests
----------------------------------------

.. test-case:: Overweight BMI
   :id: T_overweight
   :file: ../../software/bmi/report.xml
   :suite: pytest
   :classname: test_bmi_calculator.TestBMICalculator
   :case: test_bmi_overweight
   :links: I_user_friendly, R_user_friendly
   
   A pytest test case to test overweight.


Test Results of automated tests
--------------------------------------

.. test-results:: ../../software/bmi/report.xml




