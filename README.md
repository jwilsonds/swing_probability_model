# swing_probability_model
This is the code for my swing probability model that I talk about in my article on Medium.

## Analysis Summary
This model attempts to determine whether or not an MLB hitter will swing at a given pitch. I trained the model using pitch-by-pitch data from StatCast and 
used the following features: pitch speed, pitch location, the velocity in the x,y,z, directions, the count the pitch was thrown in, the movement of the 
pitch in the x,z directions, and the pitch type of the previous pitch. I then used the predicted probabilities that the model gave to make a hexbin plot
to show what locations had the highest probability of being swung at. 
## Data Source
The data used to train the model was gathered using the pybaseball library which scrapes pitch-by-pitch data from Fangraphs and Baseball Savant
## Applications
I think this model could be applied effectively in many ways. One use for it could be to enhance pitcher's scouting reports on hitters
By using the individual pitcher's average pitch movement/speed, the model can predict the hitter's behavior with relative accuracy even if he has never 
faced that pitcher before. This can help make scouting reports that are tailored to a specific pitcher and provide insight into the batter's behavior that 
would otherwise be left undiscovered.
Secondly, this model could also be used in simulations that try and predict how well a batter or pitcher will do in a game. Using a model like this one to 
predict swing probability alongside other algorithms to predict swing outcomes could be helpful in predicting the result of an at-bat against a specific 
pitcher.
