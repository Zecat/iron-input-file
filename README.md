# iron-input-file

*with Polymer 1.0*

iron-input-file extends the native input element and 
gives it an Api.

This element provides a convenient way to use an hidden input type="file" without having to bind the 'click' event manually and gives you the opportunity to modify files array.

To use it, just gives it an id and use the methods it provides. The element exposes the chosen files in the bindFiles attribute.

Don't directly bind to 'value' or 'files' attribute, for security reasons, browsers does not allow us to manipulate them as we please. To use it in a form, create a custom element wrapping iron-input-form and implementing IronFormElementBehavior, and use this custom element in an iron-form.

Example:

    <input is="iron-input-file">
