# Ocean-Wave-Prediction-Model-with-LSTM
Deep learning application for predicting ocean wave behaviors.
Predicting wave behaviors is an important tool for the safety of ship navigation and offshore operations.

In order to predict wave behaviors we need to collect wave data. Wave monitoring buoys are used for collecting the data. Wave monitoring buoys continuously measures the wave height, wave period and wave direction.

As the wave monitoring buoy floats up and down each passing wave, its motion is measured and electronically processed. Data from the wave monitoring buoys are transmitted to a nearby receiver station as a radio signal.

Measured and derived wave data in this study is collected by oceanographic wave measuring buoys anchored at Mooloolaba/Queensland/Australia.

My aim is to create a Long Short Time Memory (LSTM) deep learning model to predict future wave behaviors. In order to achive this I will divide the data set into two part (train and test). Every 30 samples from the training data will be investigated and the 31st sample features will be predicted by the model. Once the model is properly trained, test data will be used as real time wave data. And lastly I will compare these real data samples and my model's predictions to evaluate the model's success.

The wave data used in this study contains following features:
* Date/Time: Date and 30 minute wave record
* Hs : The significant wave height (in metres), defined as the average of the highest one-third of wave heights in a 30 minute wave record.
* Hmax: The height (in metres) of the highest single wave in a wave record.
* Tz: The average of the zero up-crossing wave periods (in seconds) in a wave record.
* Tp: This is the wave period (in seconds) of those waves that are producing the most energy in a wave record.
* Peak Direction: The direction that peak waves are coming from, shown in degrees from true north.
* SST: The sea surface temperature at the wave monitoring buoy, in degrees Celsius.

## References:
https://www.qld.gov.au/environment/coasts-waterways/beach/monitoring/waves

https://www.data.qld.gov.au/dataset/coastal-data-system-waves-mooloolaba

https://www.kaggle.com/jolasa/waves-measuring-buoys-data-mooloolaba
