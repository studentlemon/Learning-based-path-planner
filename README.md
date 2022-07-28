# Learning-based-path-planner

This is the open-source code for the article: Trajectory Planning for Autonomous Driving in Unstructured Scenario with Learning-based Network and Optimization method. The repo mainly includes two module: path planning and speed planning.


Path planning:

1. The enviroment is running on Python 3.7 with pytorch 1.2. If developer has not pytorch, it's recommended that you use the ground truth generated by A*, which can run directly.
command: 
       python gui.py 

2. The training network is located in segmentation networks which developers can test the performance of prediction. You can train and eval by yourself.
run: 
      python main_nagivation_prediction.py

Note that due to the business cooperation, the open-source code of path planning is rebuiled on Python. Its running speed will be lower than the C++ version. Interested developers can write their own according to the open source code. 


Speed planning:
      In order to visually show the effect of vehicle speed planning, the related program is integrated in the Qt with C++. 
      Dependency:  
      1. osqp 0.4.0 (Pay attention to the version, otherwise an error will be reported);
      2. Qcustomplot.
