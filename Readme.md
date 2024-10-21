This project intends to showcase the use of LLMs for analyzing sentiments of earning calls' audio files of AMZ and leverage it for trading amz stock

Technical Aspects
    1. AMZ Audio files were transcribed into transcripts using Open AI whisper Model
    2. The transcribed text for further cleaned to remove irrelevant textual information
    3. The transcripts were broken down into 1 minute timestamps to analyse the price movement during the meetings.
    4. Using Finbert the rolling sentiment score were calculated and with 0.1 as our threshold, 
                      if the rolling sentiments were greater than 0.1 then we take a long position in the stock 
                   else we take a short position
    5. We close our position by the end of the meeting


Use Cases
    1. Applying this approach across Fortune 500 Companies can help traders leverage price changes due to sentiments associated during the earning call


Risks 
    1.  Usually CEOs will tend to be positive during the  earning call irrespective of  the company's  performance.
    2.  Trades may not be executed in real time manner.
Mitigations 
    1.  Use cloud based trading platforms to implement real time data fetches and time executions
    2.  Augmenting the stratgies along with company financial data and moving average strategies can improve the accuracy of the trade
    3.  If video of the meeting is offered, then meeting memeber's facial expressions, eye movements, dressing pattern and other key indicators might lead to hints as to how the stock is performing or will perform. Augementing these data along with Statistical Machine learning and sentiments can lead to a robust strategy.

