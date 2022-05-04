# Surfs Up!
## Overview
I am working with W. Avy to convince him that a ice cream / surf shop in Oahu, HI is a worthwhile investment. W. Avy is interested, but he has some concerns regarding how profitable a shop of this nature can be year round. Avy's main concern is how the weather in Oahu mayu impact my store's success. So, W. Avy has a requested a statistical analysis of the weather in Oahu, specifically in the months of June and December.

## Results
![June_Stats](https://user-images.githubusercontent.com/99751636/166503451-67dca6a5-693f-46ff-968d-c206f71839b5.png)
![December_Stats](https://user-images.githubusercontent.com/99751636/166503463-b72d230c-3f34-4e16-b7c3-2e55526b87f0.png)

* June has a higher mean temperature than December
* December has a slightly highder StDev, thus it's weather fluctuates a little more.
* Both months nearly have the same max temperature, but December's minimum temperature is almost 10 degrees less than June's.


## Summary
We can see that the weather in June is both warmer and more consistent than the weather in December, as is shown by June's higher mean temperature and lower standard deviation. This does not mean the weather is unbareable in December, however. With a mean temperature of 71 degrees and a maximum temperature of 81 degrees, December conditions appear to be suitable for ice cream and surfing. If we wanted to go a step further, however, I would recommend adding the temperature for our missing seasons. Right now we can see the beginning of summer (June) and winter (December) but how does the weather looks in the beginning of spring and autumn?

session.query(Measurement.tobs, Measurement.date).filter(extract('month', Measurement.date) == 3).all()
session.query(Measurement.tobs, Measurement.date).filter(extract('month', Measurement.date) == 9).all()
