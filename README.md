# MooveeProjectDemos


The system is consisted of two pipelines: visual and radar.
In the visual pipeline, the object information is captured via a calibrated IP-camera and is then detected by a deep-learning-based one-shot object detector.
In the radar pipeline, the object is recognized via an integrated mmWave radar module. The object information captured from radar is then analyzed and filtered to counter multi-path effect.

The object-level information from both pipelines is feed into a Kalman-filter-based data aggregator, which eventually present the fusion result to the user. 

The overall latency is lower than 100ms and can achieve real-time performance for 2-way 720P security camera on an Nvidia TX2 Jetson evaluation board.
