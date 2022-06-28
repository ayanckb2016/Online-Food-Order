This is a Python-based project, where real-time object detection from the integrated webcam is performed. That is by execution of the code, a web url will be generated. The url has to be copied and pasted in the web browser and then the webcam will be activated and real-time object detection will start. The project utilizes Flask framework as web tool and OpenCV for the object detection purpose.

App

The project is deployed on Heroku. Following is the link to the Heroku-api of the project https://live-object-detection.herokuapp.com/

Dependencies

pip install requirements.txt
Arguments

*\directory>  python app.py -h/--help
usage: app.py [-h] [-wt MODEL_WEIGHTS] [-cfg MODEL_CFG] [-cls DATASET_CLASSES] [-is_realtime] [-vid VID_PATH] [-fd FRAME_DIMENSION]
              [-conf_threh THRESHOLD_CONFIDENCE] [-p PORT] [-hst HOST] [-is_dbg]

Object detection with OpenCV

optional arguments:
  -h, --help            show this help message and exit
  -wt MODEL_WEIGHTS, --model_weights MODEL_WEIGHTS
                        Path to the pre-trained weights of the network
  -cfg MODEL_CFG, --model_cfg MODEL_CFG
                        Path to the .config file of the network
  -cls DATASET_CLASSES, --dataset_classes DATASET_CLASSES
                        Path to the classes file of the dataset
  -is_realtime, --is_realtime
                        Is real time object detection is being performed
  -vid VID_PATH, --vid_path VID_PATH
                        Path to the video file
  -fd FRAME_DIMENSION, --frame_dimension FRAME_DIMENSION
                        The dimensions of the frames
  -conf_threh THRESHOLD_CONFIDENCE, --threshold_confidence THRESHOLD_CONFIDENCE
                        Threshold confidence for selecting an object
  -p PORT, --port PORT  The port of the server
  -hst HOST, --host HOST
                        The host
  -is_dbg, --is_debug   Is debugging be performed during the app run
Run

*\directory> python app.py
