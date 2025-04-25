# Sketchify – A Quick, Draw! drawing classifier
The project focuses on classifying digital drawings or doodles by identifying the object or category they represent.

## Dataset:
The [Quick Draw Dataset](https://quickdraw.withgoogle.com/data) is a collection of 50 million drawings across 345 categories, contributed by players of the game [Quick, Draw!](https://quickdraw.withgoogle.com/). It has been compiled by Google Creative Lab to help developers train new neural networks, help researchers see patterns in how people around the world draw, and help artists create things we haven’t begun to think of.

The [simplified dataset](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/simplified;tab=objects?invt=AbvrVA&prefix=&forceOnObjectsSortingFiltering=false) consists of drawings recorded as timestamped vectors, tagged with metadata. It includes the following features: word (category of the drawing), countrycode (player's country), timestamp, recognized (indicating whether the model successfully classified the drawing), key_id, and the drawing array. The drawing array contains x and y pixel coordinates and t, which represents the time in milliseconds since the first point. The dataset has 345 output classes, each representing a distinct drawing category, i.e. the object that has been drawn.
