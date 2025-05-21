Check Your Understanding
Authors: Gautam Mohandas and Eric Wang
1) I would fit my automated tests as a Github action that runs whenever code is pushed (1) because the debugging and functionality is implemented through deploying the server locally, which makes testing locally a little repetitive. However, adding a linter and tester after a push would catch on the things that a human didn't pick up on.
2) Yes, I would use an end to end test to check if a function is returning the correct output, since the input of the function will be what the user inputs, and an end to end test makes sure that the user input outputs the wanted output.
3) Difference between Navigation Mode and Snapshot Mode:
Navigation mode analyzes a page after a full page load. By opening up the URL in a new tab it does a full analysis from the start of the load based on the categories selected and separates itself from the snapshot mode by giving an outlook into the performance during the load.
Snapshot mode on the other hand just like its name sort of freezes the page in time and analyzes it based on its current state. It doesn’t “grade” the site on performance as the analysis isn’t based on load. While it does still seem to track non-load based performance metrics like missing tags it doesn’t contribute to its score.
4) Three Things to Improve:
1. Load times seem to be taking a hit from the images and the way they are stored/loaded as seen in the LCP diagnostic fails. Optimizing images for either smaller file sizes or preloading them can be ways to fix this issue. We can also use next-gen formats to serve images.
2. In the mobile version of the test the missing viewport tag will cause accessibility and visibility issues as it won’t be a responsive page. Making sure to add this will allow users to see a scaled version of the page instead of having to zoom in.
3. Lastly, there seems to be incorrect caching structure that increases load when repeatedly visiting the site. Making sure that we cache static assets will allow us to reduce this overhead.

