What is a Django model?

Django models are sources of information and behaviors stored within a single database table.

 

How does a Django model work?

Think of a Django model as a blueprint.

Each model is comprised of Django model fields that require user input.

Once the user completes the required fields, a model object is saved in the database.

The model's information is then accessible via a queryset, a callable collection of the model objects.

Are Django models required?

Django models are technically not required but are highly recommended.

It is good practice to use Django models whenever possible to minimize repetitive code but are ultimately not required for 

for unchanging or rarely changing site information.

The Django admin site
One of the most powerful parts of Django is the automatic admin interface. It reads metadata from your models to provide a quick, model-centric interface where trusted users can manage content on your site. The admin’s recommended use is limited to an organization’s internal management tool. It’s not intended for building your entire front end around.

The admin has many hooks for customization, but beware of trying to use those hooks exclusively. If you need to provide a more process-centric interface that abstracts away the implementation details of database tables and fields, then it’s probably time to write your own views.

In this document we discuss how to activate, use, and customize Django’s admin interface.

