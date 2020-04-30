## Workout Tracker

## Description

This is a simple application to keep the track of your daily workouts, providing a multifaceted analysis of those workouts for you to see in terms of duration and weight lifted in the case of resistance exercise.

The workout tracker is deployed to Heroku here: https://intense-ravine-40441.herokuapp.com/

## Usage

On the homepage, make a new workout by hitting the green button, or continue making the most recent workout you have started by hitting the blue button. The workout is made up of exercises under one of two categories, cardio and resistance, and they have their own characteristics as listed below:

* Duration, all
* Distance, cardio only
* Weight Lifted, resistance only
* Sets, resistance only
* Reps, resistance only

You can view the complete analysis of up to your 10 most recent workouts on the [stats page](https://intense-ravine-40441.herokuapp.com/stats).

## Credits

The workout tracker app uses [Express](http://expressjs.com/) to create the server and [mongoose](https://www.npmjs.com/package/mongoose) to create the MongoDB database/workout model and perform queries on the database.

The [mLab MongoDB](https://devcenter.heroku.com/articles/mongolab) Heroku add-on hosts the MongoDB database used by the deployed app on the cloud.

[Chart.js](https://www.chartjs.org/) is used to create the visual representations of workout stats with Canvas API, and the [moment.js](https://momentjs.com/) JS library prints the dates in the specified format on the `stats` page.

The frontend of this project was completely written by the Coding Boot Camp at UT using the [Bootstrap](https://getbootstrap.com/) CSS framework. The Mongoose model files in `/models` and the API routes in `server.js` are newly written to make the whole app work based on the starter code, and the new code in `stats.js` has been written to integrate with the starter code to produce the analysis of workouts in a specific time range based completely on the user's input.

## License
Copyright (c) Angela Li. All rights reserved.
Licensed under the [MIT License](LICENSE).