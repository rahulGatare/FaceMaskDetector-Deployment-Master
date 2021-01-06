## ML-Model-Flask-Deployment
This is a demo project to elaborate how Deep Learning Models are deployed on production using Flask API

### Prerequisites
You must have Scikit Learn, Pandas, Tensorflow (for Machine Leraning Model) and Flask (for API) installed.

### Project Structure
This project has four major parts :
1. deploy.prototxt and res10_300x300_ssd_iter_140000.caffemodel used for face detection
2. "mask_detector.model" used for mask detection
3. app.py - This contains Flask APIs.After button click face detection and mask detection models get loded and by using imutils and opencv opening webcam and image processing happens. 
4. templates - This folder contains the HTML template.

### Running the project

1. Run app.py using below command to start Flask API
```
python app.py
```
By default, flask will run on port 5000.

2. Navigate to URL http://localhost:5000

You should be able to view the homepage as below :
![alt text](http://www.thepythonblog.com/wp-content/uploads/2019/02/Homepage.png)

Enter valid numerical values in all 3 input boxes and hit Predict.



3. You can also send direct POST requests to FLask API using Python's inbuilt request module
Run the beow command to send the request with some pre-popuated values -
```
python request.py
```
