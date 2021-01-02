# Django

![](https://pythondevs.org/wp-content/uploads/2020/05/1562632_a245_2.jpg)

## The model layer

* Django provides an abstraction layer (the “models”) for structuring and manipulating the data of your Web application. 

### Fields¶

* The most important part of a model – and the only required part of a model – is the list of database fields it defines.

### Field types

* Each field in your model should be an instance of the appropriate Field class. Django uses the field class types to determine a few things:

  * The column type, which tells the database what kind of data to store ` INTEGER, VARCHAR, TEXT`.
  * The default HTML widget to use when rendering a form field ` <input type="text">, <select>`.
  * The minimal validation requirements, used in Django’s admin and in automatically-generated forms.

### Field options

* Each field takes a certain set of field-specific arguments (documented in the model field reference)

### Automatic primary key fields

* By default, Django gives each model the following field:

  * `id = models.AutoField(primary_key=True)`

### Verbose field names

* Each field type, except for ForeignKey, ManyToManyField and OneToOneField, takes an optional first positional argument – a verbose name.

* If the verbose name isn’t given, Django will automatically create it using the field’s attribute name, converting underscores to spaces.

### Models across files

* It’s perfectly OK to relate a model to one from another app. To do this, import the related model at the top of the file where your model is defined. Then, refer to the other model class wherever needed

### Field name restrictions

* Django places some restrictions on model field names:

  * A field name cannot be a Python reserved word, because that would result in a Python syntax error.
  * A field name cannot contain more than one underscore in a row, due to the way Django’s query lookup syntax works
  * A field name cannot end with an underscore, for similar reasons.

### Custom field types

* If one of the existing model fields cannot be used to fit your purposes, or if you wish to take advantage of some less common database column types, you can create your own field class.
* Full coverage of creating your own fields is provided in Writing custom model fields.

