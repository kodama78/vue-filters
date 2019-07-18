# vue-filters

#### Filters
* filter - helps you transform output of your data
* filter functions always have a `value` argument that is the value that they are being passed
* Uses the `| ` like Angular 2 to apply a filter function to the data in the DOM element
    * the filter function must return a value

#### Computed Properties
* Look at the `input` and `li`. Think of this as a search where you input a character and it searches the array
for that fruit
* this is extremely inefficient because it will constantly cause a re-render even if not needed
* using a `computed property` is more performant than using a `filter`. They can also be better tuned to 
suit your needs

#### Mixins
* mixins look like they allow data sources, helper functions to be used in multiple components
* makes code more reusable
* code will merge them the other Vue object keys w/ the mixins

#### Global Mixin
* can be added to all parts of your app
* each component gets a copy of the object, not the original object
* updating the mixin in one component will not affect other instances of the same mixin
* if you want to make the updating global, you could add it to the Vue object

