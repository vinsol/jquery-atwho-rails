### Usage
---
Bind your textarea

```javascript
$(function(){
    data = ['tom','john'];
    $('textarea').atwho({at:"@", 'data':data});
});
```

that's it, check it out!
more details in [At.js Home Page](http://ichord.github.com/At.js/)

### Overrites
1. Added "stopPropagationOnEnter" flat to stop event propagatoin on enter
2. Handle '.' when showing highlighted results

### Installation
---
#### Rails 3.0.x
Issue command line bellow:  
`rails generate atwho:install`  
then It will show in `public/[javascript|stylesheets]/` directory.

#### Rails >= 3.1.x
Add this gem in `Gemfile` like this:

```ruby
gem 'jquery-atwho-rails'
```

add in `app/assets/javascripts/application.js`:

```
//= require jquery
//= require jquery.atwho
```

and in `app/assets/stylesheets/applications.css`:

``` 
//=require jquery.atwho
```

#### History Versions 
All in [At.js](https://github.com/ichord/At.js) project.

### Development
---
#### Test generator
Just issue  
`bundle` then `appraisal rails30 rspec`
