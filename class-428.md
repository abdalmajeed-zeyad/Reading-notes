Django Forms

Django provides a Form class which is used to create HTML forms. It describes a form and how it works and appears.

It is similar to the ModelForm class that creates a form by using the Model, but it does not require the Model.

Each field of the form class map to the HTML form <input> element and each one is a class itself, it manages form data and performs validation while submitting the form.

Lets see an example, in which we are creating some fields too.

from django import forms  
class StudentForm(forms.Form):  
    firstname = forms.CharField(label="Enter first name",max_length=50)  
    lastname  = forms.CharField(label="Enter last name", max_length = 100)  
A StudentForm is created that contains two fields of CharField type. Charfield is a class and used to create an HTML text input component in the form.

The label is used to set HTML label of the component and max_length sets length of an input value.

When rendered, it produces the following HTML to the browser.