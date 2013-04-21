# Ember.PageableMixin

Provides interface for pagination over Ember ArrayController data:

```js
App.myController = Ember.ArrayController.create(Ember.PageableMixin);

// add content

// initialize page settings
App.myController.set('pageNumber', 2);
App.myController.set('pageSize', 10);
```

```handlebars
{{#each item in myController}}
    <!-- only iterates over values in page 2 of collection, i.e. values from index 20 to 30 -->
{{/each}}
```
