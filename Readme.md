# Stock Movement Using State-of-the-art Transformer Model

## Introduction
Deep learning plays a crucial role in many
fields, including computer vision, self-driving cars,
behavior analysis, natural language processing (NLP),
and medicine, to name a few. The financial sector comes
as no surprise where deep learning is used extensively.
The Transformer Neural Network model is one of the
most novel advancements in the sector of Deep Learning
and Machine vision. In this research paper we use the
Transformer architecture to predict Closing Price rise
and fall on the Amazon (AMZN) dataset. Analyzing this
time series, we predict our evaluation metrics in the form
of a rising and falling plot and consider evaluation errors
if any. The application of this Transformer model in the
near future would be explosive considering the fact that
today’s world is shifting towards ‘algorithmic trading’ as
a whole. Considering the Amazon (AMZN) timeseries
dataset in this paper we have solely made and
demonstrated a comparison as to why the Transformer
model once used only in Natural language processing
applications is highly beneficial in these non- linear
pattern prediction applications in the FinTech domain.
The applicability and usefulness of our model is
demonstrated by its ability to predict mid prices with a
significant probability rate. Our work on this dataset
would significantly encourage the fintech domain to adopt
the ‘transformer deep net’ model.

## Literature Survey
Not long ago, several forecasting professionals condemned
neural networks (NN) as being unsuitable and uncompetitive
in forecasting sectors. Because of its tremendous
volatility, the stock market is a new topic for academics,
students, traders, investors, and corporations. It is now
feasible to anticipate the market to some level thanks to the
amount of processing power and methodologies that have
been created. Sentiment analysis plays a vital role in the
markets. Sousa et al used CNN and BERT (Bidirectional
Encoder Representations from Transformers) in research and
discovered that for sentiment analysis, BERT would be a
better choice than CNN. Similarly, Li et al have used
BERT, LSTM (Long Short Term Memory) and Support
Vector Machines for sentiment analysis in the stock market.
The typical neural machine translation technique that
competes with and occasionally exceeds traditional statistical
machine translation techniques is the encoder-decoder
architecture for recurrent neural networks. The models giving
optimum performance bridges the encoder and decoder
through an attention mechanism as introduced by Vaswani et
al. Self-attention layers are present in the encoder. All of
the keys, values, and queries in a self-attention layer originate
from the same source, in this example, the encoder's output
from the previous layer. Each position in the encoder has
access to every position in the previous layer. Long-range
dependencies are no longer a concern since attention makes

it easier to connect any two elements of the sequence. Long-
range dependencies have the same chance of being taken into

consideration with transformers as any other short-range
dependencies. We have chosen the Amazon (AMZN) dataset
consisting of 2640 days from 12th January 2011 to 09th July
2021.

## Dataset
The data set is obtained from Yahoo financial services.
The pre-processed data set contains date, opening, closing,
high, low , volume traded per day and adjusted closing prices.
Pandas are used to convert csv to columns. The data is dated
from 12th January 2011 to 09th July 2021. The data set is
unclean and a few values have been corrupted so the data is
cleaned and normalized.

## Data Preprocessing
Data of Amazon (AMZN) share price and its daily movement
have been used as inputs for training, testing and validation.
We have used the opening and closing values to find averages
and used to compress the amount of data. the data is split into
train, validate and test subsets in the ratio of (70,20,10)
respectively. The data is reshaped to fit to be put through the
transformer header. Scaling to keep the shape and original
features of the transform but restrict the values in between the
normalized values of 0 to 1 for using activation functions such
as sigmoid. Also normalization leads easily updating of
weights and biases in the feed-forward and feed-backward
propagations. Exponential smoothing is applied to data to
reduce the weight of older data and increase the weight of
more recent data and smoothening.

## Modelling
The processed data
is used to train the Transformer Model. The special features
of the model are self attention, multi head attention, position
wise feed-forward, Bi-directional LSTM. All
hyperparameters are set to optimize the training and make
best use of the available resources. After training is validated
and mean square error is used to analyse the results. The results are compared to ARIMA and LSTM models as well to see how well transformers perform as compared to the traditional models used for time series data

## Results
| Model type | MSE |
| --- | --- |
| `Transformer` | 0.0004091 |
| `ARIMA` |  0.0004791  |
| `LSTM` |  0.0004397  |

We evaluated the models through various parameters after training and testing the validated score of
MSE was obtained for the given Amazon Stocks Time series
dataset. The training and evaluation demonstrated that the
suggested model architectures sufficed for identifying
complex patterns in financial time series irregularities. 

## Conclusion
The closing-price of Amazon (AMZN) stocks are predicted
and plotted with the actual closing-price. We attained the
actual closing parameter value trend and the predicted close
price value trend very close to each other. Therefore, the
transformer model on the given dataset of Amazon (AMZN)
works well and the result obtained is as desired.


## Note:
This code was uploaded and tested on AMZN dataset in order to compile a technical report on State of the art Transformer model. In no way is this code owned by the repsective repository owner. Happy Coding !
