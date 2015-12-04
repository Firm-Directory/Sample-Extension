# Sample-Extension
The **Firm Directory Extension Framework** is a JavaScript-based framework that allows developers to extend the core capabilities of the Neudesic Firm Directory platform to deliver new functionality.

To access most of the framework functionality, you will be writing JavaScript using functions in the `pulse.extensions` namespace. This namespace is also aliased as `pex` and you can use either interchangeably. The examples in this documentation will be using the `pex` convention for brevity, however, if you prefer, you can replace this with `pulse.extensions`.

For example, to add a new menu item to the People menu, that navigates directly to the Advanced People Search screen you would use the following JavaScript:

```
pex.addMenuItem({
   position: 'bottom',
   existingMenu: pex.menus.people,
   id: 'menu-advanced-people-search',
   text: 'Advanced People Search',
   url: '/streams/people?view=advanced'
});
```
