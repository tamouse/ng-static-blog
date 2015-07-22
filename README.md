# Angular Static Blog

Based upon [@henderixer](https://github.com/Hendrixer)'s
[ngBlog](https://github.com/angular-class/ngBlog) which we used in
[FrontendMaster](https://frontendmasters.com/) course
[Angular Components and ES6](), I thought this might be a cool way to
marry up [Jekyll](http://jekyllrb.com) with Angular in a different
sort of way.

This repo also makes a pretty dandy starter kit for a componented
Angular app all by itself. I'll probably stash that off in a branch
before I start integrating Jekyll.

## Dependencies

Install these globally

* node (~> 0.12)
* npm
* gulp
* karma
* karma-cli
* json-server

## Develop and Test

### Start up `json-server`

    $ json-server -p 3030 -H 0.0.0.0 -w db.json

The port 3030 can be modified (but should always match) the port given
in `client/app/shared/api.js` `url` field.

### Run `gulp`

    $ gulp

The default `gulp` task will compile all the application bits and
serve them up on port 4500.

The port is set in `Gulpfile.js`.
