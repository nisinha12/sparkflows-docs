Reports
=======================

Fire allows you to create dashboards.

Processors in Fire can output data in tables, charts, maps and simple strings. Dashboards allow combining of the output of various processors into one User Interface.

For example, we might want to output a chart of the number of bike rentals per hour, another by per day and another map displaying the total number of bike rentals per city for the day. Dashboards can combine all these into one view.
 
Creating Dashboards
--------------------
 
- For creating dashboards, drag and drop the required processors from the workflows into the Dashboard Canvas.
- When the corresponding workflows are run, the output is stored by Fire into the relational store. These get displayed in the dashboard.
 
Editing Dashboards
------------------

Editing dashboards is like creating dashboards, except that you click the edit button to edit the corresponding dashboard.
 
.. figure:: ../../../_assets/user-guide/dashboard-edit.png
   :alt: Sparkflows Editing Dashboards
   :width: 90%
   
   
Viewing Dashboards
------------------

Once a dashboard has been created, you can view it by clicking on the 'View' button.
  
.. figure:: ../../../_assets/user-guide/dashboard-view.png
   :alt: Sparkflows Dashboard
   :width: 90%
   
Streaming Dashboards
---------------------
 
- Fire allows you to create streaming workflow.
- The streaming workflows have a mini-batch duration, say 30 seconds.
- In this case, the output in the dashboards gets updated every 30 seconds as the new data comes in.



